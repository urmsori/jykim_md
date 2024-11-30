# 설치/실행
## WSL Docker를 이용한 실행방법
docker run -it --rm -e DISPLAY=$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix antmicro/renode

### 특정 폴더를 Workspace로 해서 실행
docker run -it --rm \
    -e DISPLAY=$DISPLAY \
    -v /tmp/.X11-unix:/tmp/.X11-unix \
    -v $PWD:/opt/renode/workspace \
    antmicro/renode