# node-red-contrib-signal-counter

This is a  Node-RED node that counts messages passing through it. 

## Description

The `signal-counter` node is an easy way to monitor and count the flow of messages in your Node-RED applications. Each time a message passes through this node, it increments a counter and sends the message as a JSON payload which includes the message's payload, topic, and the current count. If the node receives a message with the topic 'resetCounter', it resets the counter to 0. If it receives a message with the topic 'msgCount', it sends a message with the count value in the payload. 

The current count value is also displayed in the node status in the Node-RED editor.


## Installation

To install this node, you can either install it from the Node-RED palette manager or run the following command in your Node-RED user directory (typically `~/.node-red`):

```bash
npm install node-red-contrib-trexmes-signal-counter
```

## Usage

Once the node is installed, it will appear in the Node-RED palette. You can then drag and drop it onto your flow canvas. Any messages that pass through the node will increment the counter and be enriched with a `count` property.

## Author

- Asaf Yurdakul - [GitHub](https://github.com/asafyurdakul)

## License

This project is licensed under the GPL-3.0 License - see the [LICENSE](LICENSE) file for details.

