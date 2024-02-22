cmake_minimum_required(VERSION 3.20.0)
project(rtsp_server)

# rtsp测试代码
add_executable(test_rtsp
test_rtsp.c
)

# rtp h264测试代码
add_executable(test_rtp_h264
rtp_h264.c
rtp.c
)

# rtp aac测试代码
add_executable(test_rtp_aac
rtp_aac.c
rtp.c
)

# rtsp h264 server测试代码, rtp over udp
add_executable(h264_rtsp_server
h264_rtsp_server.c
rtp.c
)

# rtsp aac server测试代码
add_executable(aac_rtsp_server
aac_rtsp_server.c
rtp.c
)

# rtsp multicast server测试代码
add_executable(multicast_rtsp_server
multicast_rtsp_server.c
rtp.c
)

# rtsp server测试代码, rtp over tcp
add_executable(tcp_rtsp_server
tcp_rtsp_server.c
tcp_rtp.c
)