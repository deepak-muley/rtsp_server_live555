https://github.com/vimagick/dockerfiles/tree/master/live555
sample videos downloaded from http://www.live555.com/liveMedia/faq.html#264-file

To access the rtsp stream use following:
<pre>
$ docker-compose up --build
Pulling rtsp_server_live555 (vimagick/live555:)...
latest: Pulling from vimagick/live555
63bc94deeb28: Pull complete
c2a4251c2e63: Pull complete
8080b342fa67: Pull complete
Digest: sha256:a94c955b969386721f767abbb76a6daa9d227c80fee8c34720a9fe4c51a87bd5
Status: Downloaded newer image for vimagick/live555:latest
Creating rtsp_server_live555_rtsp_server_live555_1 ... done
Attaching to rtsp_server_live555_rtsp_server_live555_1
rtsp_server_live555_1  | LIVE555 Media Server
rtsp_server_live555_1  | 	version 0.90 (LIVE555 Streaming Media library version 2017.05.29).
rtsp_server_live555_1  | Play streams from this server using the URL
rtsp_server_live555_1  | 	rtsp://172.17.0.2/<filename>
rtsp_server_live555_1  | where <filename> is a file present in the current directory.
rtsp_server_live555_1  | Each file's type is inferred from its name suffix:
rtsp_server_live555_1  | 	".264" => a H.264 Video Elementary Stream file
rtsp_server_live555_1  | 	".265" => a H.265 Video Elementary Stream file
rtsp_server_live555_1  | 	".aac" => an AAC Audio (ADTS format) file
rtsp_server_live555_1  | 	".ac3" => an AC-3 Audio file
rtsp_server_live555_1  | 	".amr" => an AMR Audio file
rtsp_server_live555_1  | 	".dv" => a DV Video file
rtsp_server_live555_1  | 	".m4e" => a MPEG-4 Video Elementary Stream file
rtsp_server_live555_1  | 	".mkv" => a Matroska audio+video+(optional)subtitles file
rtsp_server_live555_1  | 	".mp3" => a MPEG-1 or 2 Audio file
rtsp_server_live555_1  | 	".mpg" => a MPEG-1 or 2 Program Stream (audio+video) file
rtsp_server_live555_1  | 	".ogg" or ".ogv" or ".opus" => an Ogg audio and/or video file
rtsp_server_live555_1  | 	".ts" => a MPEG Transport Stream file
rtsp_server_live555_1  | 		(a ".tsx" index file - if present - provides server 'trick play' support)
rtsp_server_live555_1  | 	".vob" => a VOB (MPEG-2 video with AC-3 audio) file
rtsp_server_live555_1  | 	".wav" => a WAV Audio file
rtsp_server_live555_1  | 	".webm" => a WebM audio(Vorbis)+video(VP8) file
rtsp_server_live555_1  | See http://www.live555.com/mediaServer/ for additional documentation.
rtsp_server_live555_1  | (We use port 80 for optional RTSP-over-HTTP tunneling, or for HTTP live streaming (for indexed Transport Stream files only).)
</pre>
