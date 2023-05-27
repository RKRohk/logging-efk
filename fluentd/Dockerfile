# fluentd/Dockerfile
FROM fluent/fluentd:edge-debian
USER root
RUN gem install fluent-plugin-elasticsearch --no-document --version 5.2.3 \
    && gem uninstall --ignore-dependencies faraday \
    && gem install faraday --no-document --version 1.10.0 \
    && gem sources --clear-all \
    && apt-get purge -y --auto-remove \
    && rm -rf /var/lib/apt/lists/* \
    && rm -rf /tmp/* /var/tmp/* /usr/lib/ruby/gems/*/cache/*.gem
USER fluent