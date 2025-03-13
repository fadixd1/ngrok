rm -rf /usr/local/bin/ngrok
rm -rf ~/ngrok

wget https://bin.equinox.io/c/bNyj1mQVY4c/ngrok-stable-linux-arm64.tgz
tar -xvzf ngrok-stable-linux-arm64.tgz
chmod +x ngrok
mv ngrok /usr/local/bin/

ngrok config add-authtoken 2u6Tuq3YwVYogtxYQC2mgvn81JO_663yx6PP8THKbP1c8Zbfy

ngrok http 3333
