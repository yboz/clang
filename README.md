# dev-clang
dev image for c++ apps based on yboz/graphical


```
docker run -d --rm -v /tmp/.X11-unix:/tmp/.X11-unix \
				   -v /home/ybozkurt/.CLion2018.2/:/home/dev/.CLion2018.2/ \
				   -v /home/ybozkurt/.java/.userPrefs/:/home/dev/.java/.userPrefs/ \
				   -v /home/ybozkurt/tools:/home/dev/tools/ \
				   -v /home/ybozkurt/src:/home/dev/src/ \
				   -e DISPLAY=unix$DISPLAY \
				   dev-clang:latest \
				   /home/dev/tools/clion-2018.2.2/bin/clion.sh
```
