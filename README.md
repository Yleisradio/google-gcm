# Google Cloud Messaging

This project is a fork from https://github.com/google/gcm to support Firebase legacy API's
send endpoint at Finnish Brodcasting Company (Yle). Firebase support is implemented
and merged into Google repo's master but build artifact is not available. Build artifact
will be shared through Yle's Maven repository: https://github.com/Yleisradio/wiki/wiki/Maven-repository

Previous build definitions (driver shell script ````./build.sh```` and Ant build definition
```client-libraries/java/rest-client/build.xml```) are removed and deploy is now done simply by Maven.

## How to deploy new lib version?

Build rest client and publish build artifact to Yle Maven repository:

    cd client-libraries/java/rest-client
    mvn deploy

Before this, update project version to the ```client-libraries/java/rest-client/pom.xml```.
    
---

Google Cloud Messaging (GCM) is a service that lets developers send data from
servers to users' devices, and receive messages from devices on the same
connection. The service provides a simple, lightweight mechanism that servers
can use to tell mobile applications to contact the server directly to fetch
updated application user data. The GCM service handles all aspects of queueing
of messages and delivery to client applications running on target devices.

This project contains client libraries and samples to help developers interface
with and explore the Google Cloud Messaging APIs.

For more information on GCM, including an overview and integration
instructions, see [Cloud Messaging](https://developers.google.com/cloud-messaging/).

For help getting started with GCM, see the
[GCM Quickstart for Android](https://developers.google.com/cloud-messaging/android/start)
or the [GCM Quickstart for iOS](https://developers.google.com/cloud-messaging/ios/start).

## Support

- Google+ Community: https://plus.sandbox.google.com/communities/105153134372062985968
- Stack Overflow: http://stackoverflow.com/questions/tagged/google-cloud-messaging

If you've found an error in this project's code, please file an issue:
https://github.com/google/gcm/issues

## License

Copyright 2015 Google, Inc.

Licensed to the Apache Software Foundation (ASF) under one or more contributor
license agreements.  See the NOTICE file distributed with this work for
additional information regarding copyright ownership.  The ASF licenses this
file to you under the Apache License, Version 2.0 (the "License"); you may not
use this file except in compliance with the License.  You may obtain a copy of
the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  See the
License for the specific language governing permissions and limitations under
the License.
