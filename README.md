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

\
