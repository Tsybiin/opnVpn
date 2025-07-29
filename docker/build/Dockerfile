#FROM kylemanna/openvpn
#  # Установите необходимые пакеты, включая OpenSSH
#RUN apt-get update && apt-get install -y openssh-server
#
#   # Создайте каталог для хранения SSH-ключей \
#RUN mkdir /var/run/sshd
#
##   # Установите пароль для root (не рекомендуется для production, лучше использовать ключи)
#RUN echo 'root:your_password' | chpasswd
#
#   # Разрешите вход по SSH под root (опять же, не рекомендуется для production)
#RUN sed -i 's/#PermitRootLogin prohibit-password/PermitRootLogin yes/' /etc/ssh/sshd_config
#
#   # Укажите порт для SSH (по умолчанию 22)
#EXPOSE 22
#
#   # Запустите SSH-сервер при старте контейнера
#CMD ["/usr/sbin/sshd", "-D"]