FROM alpine:3.7

RUN sed -i -e 's/https:/http:/' /etc/apk/repositories
RUN apk add --no-cache ca-certificates

ADD karmada-scheduler /bin/

CMD ["/bin/karmada-scheduler"]
