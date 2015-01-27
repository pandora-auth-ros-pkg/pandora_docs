# PANDORA documentation repo | [Wiki](https://github.com/pandora-auth-ros-pkg/pandora_docs/wiki)

This repo is intended for documentation files such as images, UML diagrams, pdfs and more. 
If you add a UML diagram, consider uploading the original file (.zargo, .vsdx, .dia, etc) as well as images and pdfs for that diagram in order to be easily downloadable and viewable. 
In case you need to upload an image in order to use it from the wiki, you should upload that image directly to the wiki repo. 
Clone the `https://github.com/pandora-auth-ros-pkg/pandora_docs.wiki.git` repo and you will find a folder named `images` in it.

## Quick links

- [Wiki home](https://github.com/pandora-auth-ros-pkg/pandora_docs/wiki)
- [Setting up packages](https://github.com/pandora-auth-ros-pkg/pandora_docs/wiki/Setup%20Packages)
- [Coding guidelines](https://github.com/pandora-auth-ros-pkg/pandora_docs/wiki/Coding-Guidelines)

## API documentation and Jenkins builds

|       Metapackage     |                             API Documentation                             |Jenkins build|
| --------------------- | :------------------------------------------------------------------------:|:-----------:|
| pandora_common        | -                                                                         | [Job][1]    |
| pandora_data_fusion   | [Code API](http://docs.pandora.ee.auth.gr/api/pandora_data_fusion/html/)  | [Job][2]    |
| pandora_fsm           | [Code API](http://docs.pandora.ee.auth.gr/api/pandora_fsm/html/)          | -           |
| pandora_visualization | -                                                                         | [Job][3]    |
| pandora_vision        | [Code API](http://docs.pandora.ee.auth.gr/api/pandora_vision/html/)       | -           |

[1]: http://jenkins.pandora.ee.auth.gr/job/test-pandora_common/
[2]: http://jenkins.pandora.ee.auth.gr/job/test-pandora_data_fusion/
[3]: http://jenkins.pandora.ee.auth.gr/job/test-pandora_visualization/
