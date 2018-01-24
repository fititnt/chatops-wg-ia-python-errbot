# ChatOps WG: Intelligent Agent with Python / Errbot

See main project [ChatOps for non-DevOps people Working Group 2018/01](https://github.com/fititnt/chatops-wg).


## Quickstart

Draft. Ignore this now.

```bash
# https://hub.docker.com/r/rroemhild/errbot/
docker run -d \
    --name err \
    -e BOT_USERNAME=err@xmmp.local \
    -e BOT_PASSWORD=errbotpwd \
    -e BOT_ADMINS=admin@xmpp.local \
    -e CHATROOM_PRESENCE=err@conference.xmpp.local \
    -e "TZ=Europe/Berlin" \
    rroemhild/errbot

cd /alligo/code/_temp 
git clone https://github.com/rroemhild/docker-errbot.git
docker run -it \
    --name err \
    -e BOT_USERNAME=err@xmmp.local \
    -e BOT_PASSWORD=errbotpwd \
    -e BOT_ADMINS=admin@xmpp.local \
    -e CHATROOM_PRESENCE=err@conference.xmpp.local \
    -e "TZ=Europe/Berlin" \
    rroemhild/errbot

```