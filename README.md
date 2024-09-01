# specter-ransomware

![XW](https://res.cloudinary.com/dxubkzzbx/image/upload/v1725220991/Untitled_1_hymq5n.jpg)

This Python script is designed to demonstrate a sophisticated ransomware attack simulation, encompassing both encryption and decryption functionalities. The script employs various cryptographic techniques and integrates a graphical user interface to simulate a real-world ransomware scenario.
Functionality Overview

    Encryption Mechanism: The script begins by generating a symmetric encryption key using the cryptography library. This key is then encrypted with an asymmetric RSA public key and stored securely. The encryption of target files is performed using the symmetric key. Supported file types include common document, media, and archive formats, such as .docx, .pdf, .mp4, and .rar. Once encrypted, these files are appended with a .fml extension, rendering them inaccessible without decryption.

    Decryption Interface: To facilitate the simulated recovery process, the script includes a graphical user interface (GUI) built with Tkinter. This GUI provides a user-friendly interface for entering a decryption key. Upon successful key entry, the script attempts to decrypt the previously encrypted files. If the key is valid, the original files are restored by removing the .fml extension and decrypting their contents. Failure to provide the correct key results in an error message.

    Graphical User Interface: The Tkinter GUI is designed with a polished and professional appearance, featuring rounded widgets and a gradient background. The interface includes a message informing the user of the infection, an entry field for the decryption key, and a button to initiate the decryption process. This interface not only enhances the user experience but also adds a layer of realism to the simulation.

    Error Handling: Throughout the script, error handling mechanisms are incorporated to manage potential issues during file operations and cryptographic processes. This includes handling exceptions during file reading, encryption, and decryption, as well as providing user feedback through dialog boxes.

Technical Implementation

    Cryptographic Libraries: The script utilizes the cryptography library for implementing RSA encryption and decryption, as well as symmetric encryption with the Fernet class. It ensures that sensitive data is protected using robust encryption algorithms.

    File Operations: The script performs file operations, including reading and writing encrypted content, managing file extensions, and cleaning up after encryption or decryption processes.

    Image Processing: To enhance the GUI, the script employs the PIL library for creating and manipulating images. This includes generating a gradient background and displaying an image within the Tkinter interface.

Overall, this script serves as a comprehensive example of a ransomware simulation, showcasing the integration of cryptographic techniques and graphical user interfaces to simulate a real-world cyber threat scenario. It highlights the importance of secure key management and user interaction in the context of ransomware attacks.
