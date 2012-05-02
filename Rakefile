require 'rake'
require 'httparty'

task :cron do
  url = ENV['WEBHOOK']
  method = ENV['METHOD'] || "GET"

  HTTParty.send(method.downcase, url) if url
end