FROM debian:jessie
RUN apt-get update && apt-get -y install ruby git && gem install specific_install && gem specific_install -l https://github.com/elruwen/fake_sns -b feature-add-delete-messages-endpoint
CMD ["fake_sns"]

EXPOSE 9292
