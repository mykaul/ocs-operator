FROM quay.io/openshift/origin-must-gather:latest

# Save original gather script
RUN mv /usr/bin/gather /usr/bin/gather_original

# copy all collection scripts to /usr/bin
COPY collection-scripts/* /usr/bin/

RUN mkdir /templates
COPY templates /templates

ENTRYPOINT /usr/bin/gather
