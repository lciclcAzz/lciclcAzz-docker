FROM gliderlabs/alpine

MAINTAINER lciclcAzz <lciclcAzz[AT]gmail.com>

RUN apk-install bash py-pip xvfb dbus chromium chromium-chromedriver
RUN apk add --no-cache firefox-esr
RUN pip install --upgrade pip
RUN pip install robotframework
RUN pip install robotframework-selenium2library

ADD run.sh /usr/local/bin/run.sh
RUN chmod +x /usr/local/bin/run.sh

CMD ["run.sh"]