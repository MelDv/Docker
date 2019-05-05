FROM devopsdockeruh/overwrite_cmd_exercise

WORKDIR /usr/app
COPY . . 
RUN chmod +x ./start.sh

ENTRYPOINT ["./start.sh"]
CMD  ["--clock"]
