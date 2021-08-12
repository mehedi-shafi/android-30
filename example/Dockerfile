FROM android_slim
ENV APP_PATH=/app
WORKDIR /app
COPY ./ ./
RUN chmod +x .gradlew
VOLUME ["/root/.gradle"]
VOLUME ["/app/app/build/outputs/apk/"]
ENTRYPOINT ["/bin/bash", "-c", "/app/gradlew assembleDebug"]
