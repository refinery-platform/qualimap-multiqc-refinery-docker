FROM ewels/multiqc:v1.5
# (Based on python 2.7)

COPY . .
RUN pip install -r requirements.txt

ENV VOLUME=/data
VOLUME $VOLUME

ENV PORT=80
EXPOSE $PORT

CMD ./generate_report_and_serve.sh $VOLUME $PORT
