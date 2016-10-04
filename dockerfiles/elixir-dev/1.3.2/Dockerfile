FROM vagmi/elixir:1.3.2
MAINTAINER Vagmi Mudumbai <vagmi@tarkalabs.com>

RUN apk --update add erlang-crypto erlang-syntax-tools erlang-parsetools erlang-inets erlang-ssl erlang-public-key erlang-eunit \
    erlang-asn1 erlang-sasl erlang-erl-interface erlang-dev wget git && \
    rm -rf /var/cache/apk/*

RUN mix local.hex --force && \
    mix local.rebar --force

CMD ["/bin/sh"]
