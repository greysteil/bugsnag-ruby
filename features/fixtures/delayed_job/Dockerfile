ARG ruby_version
FROM ruby:$ruby_version

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

COPY Gemfile /usr/src/app/
RUN bundle install

COPY . /usr/src/app

CMD ["bundle", "exec", "rails", "s", "-b", "0.0.0.0"]
