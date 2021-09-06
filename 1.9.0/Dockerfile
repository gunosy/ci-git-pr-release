FROM ruby:2.7-alpine3.13
RUN  apk --update --no-cache add openssh git \
  && gem install -N git-pr-release:1.9.0 \
  && rm -rf /usr/local/lib/ruby/gems/2.7.0/cache/*.gem \
  /usr/local/bundle/cache/*.gem
ENTRYPOINT ["git-pr-release"]

