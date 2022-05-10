default: install

include common.mk

install:
	npm install

serve:
	npm run start

cert:
	openssl req -x509 -newkey rsa:4096 -days 397 -keyout local.key -out local.crt -subj '/CN=roll20.local/O=The Orr Group, LLC./C=US/ST=Nevada/L=Las Vegas' -addext "subjectAltName=DNS:mediasoup.roll20.local" -nodes

