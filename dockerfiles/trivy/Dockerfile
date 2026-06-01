FROM aquasec/trivy:0.71.0

ENV TRIVY_CACHE_DIR=/trivy-cache

RUN trivy image --download-db-only
RUN trivy java-db --download-java-db-only

ENTRYPOINT ["trivy"]
