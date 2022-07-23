# DevOps-Tooling-Website-Solution
In previous [Implementing Web Solution (https://github.com/Micah-Shallom/Implementing-Wordpress-Web-Solution)] I implemented a WordPress based solution that is ready to be filled with content and can be used as a full fledged website or blog. Moving further I will add some more value to my solution so that a member of a DevOps team could utilize.

In this project, I will be introducing the concept of file sharing for multiple servers to share the same web content and also a database for storing data related to the website.

## <u>Architectural Design</u>

![web_architecture](./img/3tier%20web%20application.png)

On the diagram above we can see a common pattern where several **stateless Web Servers** share a common database and also access the same files using **Network File Sytem (NFS)** as a shared file storage. Even though the NFS server might be located on a completely separate hardware – for Web Servers it look like a local file system from where they can serve the same files.

This project consists of the following servers:
 - Web server(RHEL)
 - Database server(Ubuntu + MySQL)
 - Storage/File server(RHEL + NFS server)
 

