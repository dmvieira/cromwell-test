FROM broadinstitute/gatk:4.1.8.1

RUN mkdir /opt/cromwell \
    && wget -O /opt/cromwell/cromwell.jar https://github.com/broadinstitute/cromwell/releases/download/49/cromwell-49.jar

ADD cromwell-application.conf /opt/cromwell/cromwell-application.conf
ADD cromwell_run.sh /opt/cromwell/cromwell_run

RUN chmod a+x /opt/cromwell/cromwell_run