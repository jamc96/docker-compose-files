FROM ortussolutions/commandbox:lucee5

# COPY EXTENSION LIST TO THE DEPLOY PATH
ADD http://extension.lucee.org/rest/extension/provider/full/D4EDFDBD-A9A3-E9AF-597322D767E0C949?version=12.1.0.2 /usr/local/lib/serverHome/WEB-INF/lucee-server/deploy/ojdbc7-12.1.0.2.lex
ADD http://extension.lucee.org/rest/extension/provider/full/1C9A7C34-2555-4AAA-92FBB7FC7111140C?version=2.3.1.16 /usr/local/lib/serverHome/WEB-INF/lucee-server/deploy/log-analizer.lex

# WARM UP THE SERVER WITH THE NEW EXTENSION
RUN ${BUILD_DIR}/util/warmup-server.sh