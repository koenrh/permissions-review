# frozen_string_literal: true

require 'yaml'
require 'addressable'
require 'open-uri'

desc 'Update icons'
task :update_icons do
  services = YAML.safe_load(File.open('_data/services.yml'))
  services.each do |svc|
    uri = Addressable::URI.parse(svc['url'])
    icon = open("https://api.faviconkit.com/#{uri.domain}/64")
    IO.copy_stream(icon, "images/#{svc['name'].tr('.', '_').downcase}.png")
  end
end
