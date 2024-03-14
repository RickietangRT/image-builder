FROM debian
RUN apt update -y
RUN apt install curl -y
RUN curl -fsSL https://tailscale.com/install.sh | sh
#ENTRYPOINT["tailscaled"]

# rickietang/tailscale