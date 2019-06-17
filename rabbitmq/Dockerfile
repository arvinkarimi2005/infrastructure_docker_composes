FROM rabbitmq:3.6-management
RUN apt-get update
RUN apt-get install -y unzip wget && \
wget https://dl.bintray.com/rabbitmq/community-plugins/3.6.x/rabbitmq_delayed_message_exchange/rabbitmq_delayed_message_exchange-20171215-3.6.x.zip && \
unzip rabbitmq_delayed_message_exchange-20171215-3.6.x.zip && \
mv rabbitmq_delayed_message_exchange-20171215-3.6.x.ez /plugins/ && \
rm -f rabbitmq_delayed_message_exchange-20171215-3.6.x.zip && \
rabbitmq-plugins enable rabbitmq_delayed_message_exchange