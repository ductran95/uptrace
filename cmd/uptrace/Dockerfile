FROM alpine:latest as prep
ARG TARGETARCH
RUN apk --update add ca-certificates

COPY uptrace_${TARGETARCH} /uptrace

COPY entrypoint.sh /entrypoint.sh

EXPOSE 14317 14318
ENTRYPOINT ["/entrypoint.sh"]
