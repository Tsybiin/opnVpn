#FROM kylemanna/openvpn
RUN apk update && apk add --no-cache tzdata
ENV TZ="Europe/Moscow"
RUN useradd -ms /bin/bash old_cont
RUN usermod -u 1000 old_cont \
  && groupmod -g 1000 old_cont
RUN apt-get install sudo -y
RUN usermod -aG sudo old_cont && rm /etc/localtime && ln -s /usr/share/zoneinfo/Europe/Moscow /etc/localtime
USER old_cont