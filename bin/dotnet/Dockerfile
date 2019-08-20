FROM microsoft/dotnet:2.1-sdk
# RUN mkdir -p /app
# WORKDIR /app
# RUN ["dotnet", "restore"]
# RUN ["dotnet", "build"]
# EXPOSE 80/tcp
COPY ./entrypoint.sh /
RUN chmod +x ./entrypoint.sh
# CMD /bin/bash ./entrypoint.sh
# ENTRYPOINT [ "dotnet", "watch", "run", "--no-restore", "--urls", "https://0.0.0.0:5000"]

