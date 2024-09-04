# akbar
Discord itself supports sending and receiving data over the Websocket via JSON or ETF due their realtime websocket API being built on Erlang. The ETF encoding is actually also used by the Discord client itself when communicating over Websocket, and in general is a faster more compressed representation of the data when compared to JSON.

As such, we implemented the encoding so that developers can choose for themselves which to use when dealing with Discord.

This setting is accessible via JDABuilder#setGatewayEncoding(GatewayEncoding)


