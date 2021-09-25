FROM alpine:3.7

RUN sed -i -e 's/https:/http:/' /etc/apk/repositories
RUN apk add --no-cache ca-certificates

ADD karmada-controller-manager /bin/

CMD ["/bin/karmada-controller-manager"]
