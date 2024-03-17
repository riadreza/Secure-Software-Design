# Secure Software Concepts

**General Security Concept**

From an information and software development point of view, some specific attributes are commonly used to describe the actions associated with security: confidentiality, integrity, and availability. A second set of action-oriented elements, authentication, authorization, and auditing, provide a more complete description of the desired tasks associated with the information security activity. A final term, non-repudiation, describes an act that one can accomplish when using the previous elements. An early design decision is determining what aspects of protection are required for data elements and how they will be employed.

<figure><img src="https://lh7-us.googleusercontent.com/cd409LxJho9gOWQnRfbLPQ5tVimQbwVEJuAVDeY1gJG_Cv_FyVT1NPm6yIJ9hMV37No_M27noDNTnVLCBxPYuNAIzpjb_IWLyP88xuBS5fKURajbSNGZ_M4u5ITXnjhr-QpeZMWEBMfVdPZs8L1KMw=s2048" alt=""><figcaption><p>CIA Triangle</p></figcaption></figure>

| Confidentiality                                                                 | Integrity                                                                          | Availability                                                              |
| ------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| The information is safe from accidental or intentional disclosere               | The information is safe from accidental or intentional modification or alteration. | The information is available to authorize users when needed.              |
| Example: If I send you a message, execpt you no one will undustand the message. | Example: If I send you a message, you recive exactly same message that I send you. | Example: If I want ot send you a message, you should abale to receive it. |
| Purpose: Data is not disclosed                                                  | Purpose: Data is not tempered                                                      | Purpose: Data is available.                                               |
| We can achive it by encryption                                                  | We can achive it by hashing, Digital signeture.                                    | By backup and redundent system.                                           |
| its opposite is "Disclosure"                                                    | Its opposite is "Alteration"                                                       | Its opposite is "Destruction"                                             |

**Authentication**

Authentication is the process of determining the identity of a user. All processes in a computer system have an identity assigned to them so that differentiation of security functionality can be employed. Authentication is a foundational element of security, as it provides the means to define the separation of users by allowing the differentiation between authorized and unauthorized users. In systems where all users share a single account, they share the authentication and identity associated with that account.

To verify their identity, a user can provide

•   Something you know

•   Something you have

•   Something about you (something that you are)

**Authorization**

After the authentication system identifies a user, the authorization system takes over and applies the predetermined access levels to the user. Authorization is the process of applying access control rules to a user process and determining if a particular user process can access an object. There are numerous forms of access control systems, and these are covered later in the chapter. Three elements are used in the discussion of authorization: a requestor (sometimes referred to as the subject), the object, and the type or level of access to be granted. The authentication system identifies the subject to be one of a known set of subjects associated with a system. When a subject requests access to an object, be it a file, a program, an item of data, or any other resource, the authorization system makes the access determination as to grant or deny access. A third element is the type of access requested, with the common forms being read, write, create, delete, or the right to grant access rights to other subjects.

**Accounting (Auditing)**

Accounting is a means of measuring activity. In IT systems, this can be done by logging crucial elements of activity as they occur. Concerning data elements, accounting is needed when activity is determined to be crucial to the degree that it may be audited at a later date and time. Management has a responsibility to ensure work processes are occurring as designed. Should there be a disconnect between planned and actual operational performance metrics, then it is management’s responsibility to initiate and ensure corrective actions are taken and effective. Auditing is management’s lens to observe the operation in a nonpartisan manner. Auditing is the verification of what happened on a system. Security-level auditing can be performed at several levels, from an analysis of the logging function that logs specific activities of a system, to the management verification of the existence and operation of specific controls on a system.

**Non-repudiation**

Non-repudiation is the concept of preventing a subject from denying a previous action with an object in a system. When authentication, authorization, and auditing are properly configured, the ability to prevent repudiation by a specific subject concerning an action and an object is ensured.&#x20;

**System Tenets**

The creation of software systems involves the development of several foundational system elements within the overall system. Communication between components requires the management of a communication session, commonly called session management. When a program encounters an unexpected condition, an error can occur. Securely managing error conditions is referred to as exception management. Software systems require configuration in production, and configuration management is a key element in the creation of secure systems.

**Session Management**

Software systems frequently require communications between program elements or between users and program elements. The control of the communication session between these elements is essential to preventing the hijacking of an authorized communication channel by an unauthorized party. Session management refers to the design and implementation of controls to ensure that communication channels are secured from unauthorized access and disruption. A common example is the Transmission Control Protocol (TCP) handshake which enables the sequential numbering of packets and allows for packet retransmission for missing packets; it also prevents the introduction of unauthorized packets and the hijacking of the TCP session. Session management requires additional work and has a level of overhead, and hence may not be warranted in all communication channels. User Datagram Protocol (UDP), a connectionless/sessionless protocol, is an example of a communication channel that would not have session management and session-related overhead. An important decision early in the design process is determining when sessions need to be managed and when they do not. Understanding the use of the channel and its security needs should dictate the choice of whether session management is required or not.

**Exception Management**

There are times when a system encounters an unknown condition or is given input that results in an error. The process of handling these conditions is referred to as exception management. A remote resource may not respond, or there may be a communication error—whatever the cause of the error, the system needs to respond properly. Several criteria are necessary for secure exception management. First, all exceptions must be detected and handled. Second, the system should be designed so as not fail to in an insecure state. Last, all communications associated with the exception should not leak information.

**Configuration Management**

Dependable software in production requires the managed configuration of the functional connectivity associated with today’s complex, integrated systems. Initialization parameters, connection strings, paths, keys, and other associated variables are typical examples of configuration items. As these elements can have significant effects on the operation of a system, they are part of the system and need to be properly controlled for the system to remain secure. The identification and management of these elements is part of the security process associated with a system.&#x20;

Management has a responsibility to maintain production systems in a secure state, and this requires that configurations be protected from unauthorized changes. This has resulted in the concept of configuration management, change control boards and a host of workflow systems designed to control the configuration of a system. One important technique frequently employed is the separation of duties between production personnel and development/test personnel. This separation is one method to prevent the contamination of approved configurations in production.

**Secure Design Tenets**

Secure designs do not happen by accident. They are the product of **deliberate architecture**, and **deliberate plans**, and **are structured** upon a foundation of secure design principles. These principles have borne the test of time and have repeatedly proven their worth in a wide variety of security situations. The seminal work in this area, the application of secure design principles to computer systems, is Saltzer and Schroeder’s 1975 article “The Protection of Information in Computer Systems.”

\
\
\
\
