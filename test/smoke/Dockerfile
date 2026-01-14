FROM alpine

RUN addgroup --system <group>
RUN adduser --system <user> --ingroup <group>
USER <user>:<group>


RUN apk add curl

COPY smoke-test.sh smoke-test.sh

CMD ["sh", "smoke-test.sh", "http://app:3000"]