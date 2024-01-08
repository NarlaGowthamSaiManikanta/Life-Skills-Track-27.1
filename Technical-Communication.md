# Open System Interconnection(OSI) Model
OSI model defines how data is transferred from one computer to another computer in a computer network. It is a conceptual model from the International Organization for Standardization(ISO) that provides a common basis for the coordination of standards development for systems interconnection. In a basic form, two computers are connected using a LAN Cable, the computer can be of different operating systems, here is where the OSI model comes into the picture of sharing data between them.

- The communication in the OSI model is separated into 7 different abstraction layers namely,
  1. [Physical Layer](#physical-layer)
  2. [Data Link Layer](#data-link-layer)
  3. [Network Layer](#network-layer)
  4. [Transport Layer](#transport-layer)
  5. [Session Layer](#session-layer)
  6. [Presentation Layer](#presentation-layer)
  7. [Application Layer](#application-layer)

![Image depicting the 7 layers of the OSI Model](https://cf-assets.www.cloudflare.com/slt3lc6tev37/6ZH2Etm3LlFHTgmkjLmkxp/59ff240fb3ebdc7794ffaa6e1d69b7c2/osi_model_7_layers.png)

Each layer in this model is a package of protocols.

## Physical Layer
* The Physical layer converts the binary data into a signal to transmit over the local media.
* This Layer includes the physical equipment involved in the data transfer, such as the cables and switches.
* It deals with the physical transmission of data through cables, wires, or wireless signals.
* It is concerned with things like voltage levels, timing, and data rates.
![Illustration of Physical Layer](https://cf-assets.www.cloudflare.com/slt3lc6tev37/1HQ1W5P4XAinIdM37DTu4U/900ccdceda346baf03ce8b9f977d2974/osi_model_physical_layer_1.png)
## Data Link Layer
* The Data Link Layer is similar to the network layer, except that it allows data to be transferred between two devices on the same network.
* It deals with the physical addressing. It makes a frame by assigning the sender and destination MAC Addresses to the data packets.
* It is embedded as software in the Network Interface Card(NIC) of the computer.
* It adds error-detection bits for reliable transmission.
![Illustration of Data Link Layer](https://cf-assets.www.cloudflare.com/slt3lc6tev37/3TLHavXiotb9ayyZFKECf3/9456d1c431cd71ceea7f4b407f076f11/data_link_layer_osi_model.png)
## Network Layer
* The Network layer is responsible for facilitating data transfer between two networks.
* The functions of the network layer are logical addressing, path determination, and routing.
* IP addressing done in the network layer is the logical addressing. Every computer has a unique IP address.
* It forms a data packet by assigning source and destination IP addresses to the segment so that it can reach the right destination.
* Routing is the method of transfer of data packets from source to destination with the help of IP address and Mask.
* Path Determination determines the best path for the data delivery. OSPF, BGP, and IS-IS are some protocols of path determination.
![Illustration of Network Layer](https://cf-assets.www.cloudflare.com/slt3lc6tev37/3g2Hv0frHsql5SFauJL5EG/d8cede7b6a780e63413bd86de9eee7f9/osi_model_network_layer_3.png)
## Transport Layer
* The Transport Layer is responsible for end-to-end communication between two devices.
* It controls the reliability of communication through Segmentation, Error Control, and Flow Control.
Segmentation means the division of data into smaller data units called segments.
* Each segment consists of a Port number and Sequence number.
* The Port number helps the segment reach the right application.
* The Sequence number helps the segments to be arranged in the right order.
* Flow Control looks after the amount of data being transmitted.
* Error Control looks after all the data being transferred without any errors at times of data loss or corruption using the checksum values.
* Transmission Control Protocol(TCP) and User Datagram Protocol are the protocols of this layer.
![Illustration of Transport Layer](https://cf-assets.www.cloudflare.com/slt3lc6tev37/3OlO75NcADGL3SmEADFDqd/723b8c7639c4e2e6b4febcbe7fd36e0e/osi_model_transport_layer_4.png)
## Session Layer
* The Session Layer manages the sequence and flow of events that establish and terminate network connections.
* This layer synchronizes the data transfer with checkpoints.
* It deals with the authentication and authorization of the networks.
* It ensures that the session remains open long enough to transfer all of the data being exchanged before closing it to avoid wasting resources.
![Illustration of Session Layer](https://cf-assets.www.cloudflare.com/slt3lc6tev37/29mRrgK22AqJVlg2MMlD86/34d8f4071b6cc0d3b03c93f55e4d89b7/osi_model_session_layer_5.png)
##  Presentation Layer
* The presentation layer is responsible for translation, encryption/decryption, and compression of data.
* Translation involves the conversion of Characters and numbers into bits.
* Data Compression involves the redundancy of the bits that can be lossy or lossless, which reduces the space.
* Secure Sockets Layer(SSL) is the protocol used by the Presentation Layer for the encryption of data.
![Illustration of Presentation Layer](https://cf-assets.www.cloudflare.com/slt3lc6tev37/19L86neKKT8srUkOSe4rf7/ff4c91c94a1790651df7b48433913f59/osi_model_presentation_layer_6.png)
## Application Layer
* The Application Layer is the top layer of the OSI model.
* It supplies network services to end-user applications.
* It is used by network applications like browsers to function.
* HTTP and HTTPS are the protocols used by the browsers at the Application Layer.
* The protocols of the Application Layer are the basis for many network services like File Transfer, Web Surfing, Emails, Virtual Terminals, etc.
* Some of the protocols of the Application Layer are FTP, HTTP, HTTPS, POP3, SMTP, Telenet, etc.
![Illustration Of Application layer](https://cf-assets.www.cloudflare.com/slt3lc6tev37/2rcDKpr4WLqoyAZ7GDKkyJ/7cab96402de7ac5465b86e617da3da4e/osi_model_application_layer_7.png)

With this knowledge of the OSI model and its layers, we get an overview of the functionality of the network and we can troubleshoot the issues that may arise. Along with the OSI model, there exists another model named the TCP/IP model with only four layers and it's more practical.

## References
* [OSI Model Explained YouTube video by TechTerms.](https://youtu.be/vv4y_uOneC0?si=lxEplcZ1t2pF_s0s)
* [OSI model by Wikipedia website.](https://en.wikipedia.org/wiki/OSI_model)
* [What is the OSI Model? by Cloudflare Website](https://www.cloudflare.com/en-gb/learning/ddos/glossary/open-systems-interconnection-model-osi/)
* [The Layers of the OSI Model Illustrated by Lifewire website](https://www.lifewire.com/layers-of-the-osi-model-illustrated-818017)