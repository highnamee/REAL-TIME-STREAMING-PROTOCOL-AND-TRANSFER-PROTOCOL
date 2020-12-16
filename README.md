# REAL-TIME-STREAMING-PROTOCOL-AND-TRANSFER-PROTOCOL
In modern Internet, streaming video become more and more popular. We can see its application everywhere, especially on social networks like Facebook, Zalo or online sales pages. The application layer protocols that we often see work in a request/response manner, whereby the client asks for some piece of content, the content is delivered using TCP or UDP, and then the client application can display the content to the use. But if the user needs to watch an hour video or a movie with hundreds of megabytes of capacity, HTTP or FTP is no longer suitable for download and play.

RTSP is a solution that combines TCP to control and UDP for transport. Using this protocol, file delivery can start and the client-side application can begin displaying the audio and video content before the complete file has arrived.

In this assignment, we will use RTSP to create a simple small application to examine basicly how this procol works.
## Require
### Implement:
1. the RTSP protocol in the client
2. the RTP packetization in the server
### Extend:
1. Calculate the statistics about the session. You will need to calculate RTP packet loss rate, video data rate (in bits or bytes per second), and any other interesting statistics that you can think of.
2. The user interface on the RTPClient has 4 buttons for the 4 actions. If you compare this to a standard media player, such as RealPlayer or Windows Media Player, you can see that they have only 3 buttons for the same actions: PLAY, PAUSE, and STOP (roughly corresponding to TEARDOWN). There is no SETUP button available to the user. Given that SETUP is mandatory in an RTSP interaction, how would you implement that in a media player? When does the client send the SETUP? Come up with a solution and implement it. Also, is it appropriate to send TEARDOWN when the user clicks on the STOP button?
3. Currently, the client and server only implement the minimum necessary RTSP interactions and PAUSE. Implement the method DESCRIBE which is used to pass information about the media stream. When the server receives a DESCRIBE-request, it sends back a session description file which tells the client what kinds of streams are in the session and what encodings are used.
## Report
View report.pdf for more detail
