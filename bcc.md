# 현재 디렉토리의 hello.c를 컴파일
docker run --rm -v $PWD:/work sparc-leon3-compiler hello.c -o hello.elf