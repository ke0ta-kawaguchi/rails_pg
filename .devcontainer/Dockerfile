# Make sure RUBY_VERSION matches the Ruby version in .ruby-version
ARG RUBY_VERSION=3.4.2
FROM ghcr.io/rails/devcontainer/images/ruby:$RUBY_VERSION

RUN apt-get update -qq && \
  apt-get install --no-install-recommends -y \
  default-mysql-client libjemalloc2 libvips build-essential libyaml-dev default-libmysqlclient-dev && \
  rm -rf /var/lib/apt/lists /var/cache/apt/archives
