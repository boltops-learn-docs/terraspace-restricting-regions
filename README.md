<!-- note marker start -->
NOTE: This repo contains only the documentation for the private BoltsOps repo code.
Original file: https://github.com/boltops-learn/terraspace-restricting-regions/blob/master/README.md
The docs are publish so they are available for interested subscribers.
For access to the source code, you can become a BoltOps subscriber.
See: https://learn.boltops.com

<!-- note marker end -->

# Terraspace Restricting Regions

[![BoltOps Learn Badge](https://img.boltops.com/boltops-learn/boltops-learn.png)](https://learn.boltops.com)

[![BoltOps Badge](https://img.boltops.com/boltops/badges/boltops-badge.png)](https://www.boltops.com)

An example Terraspace project to show how to restrict the regions that can be deployed:

config/app.rb

```ruby
Terraspace.configure do |config|
  config.allow.regions = ["us-west-2"]
  # config.deny.regions = ["us-east-1"]
end
```

## Usage

Uncomment the examples in `config/app.rb` and run:

    AWS_REGION=us-west-2 terraspace up stack1
    AWS_REGION=us-east-1 terraspace up stack1

## Video

[![Watch the video](https://uploads-learn.boltops.com/w0gh4hfn2pu3p07j71y8wc6jhgkm)](https://learn.boltops.com/courses/terraspace-fundamentals/lessons/terraspace-restricting-deployment-to-allowed-aws-regions)

Note: Premium video content requires a subscription.
