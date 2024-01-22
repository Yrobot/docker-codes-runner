# docker-codes-runner
contain several docker images as the code runtime environment for different code languages.
- Typescript: [Bun.sh] - @yorbot/ts-runner
- Jar: [Java11] - @yorbot/jar-runner
- Python: [Python3] - @yorbot/py-runner

----

## How To Start
### start a ts runner

```bash
docker run -it --rm --name ts-runner -v $TS_PROJECT_PATH:/usr/src/app @yorbot/ts-runner bash
```
- `$TS_PROJECT_PATH`: the local path for ts project

inside containr:
```bash
bun index.ts
```
