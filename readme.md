Tạo model chuyển động trong gazebo, theo ví dụ:
http://gazebosim.org/tutorials?tut=actor&cat=build_robot#Scriptedtrajectories

Mô hình chuyển động gồm:
- Skeleton: các link trong model chuyển động với nhau. ví dụ tay, chân,...
- Trajectory: toàn bộ model chuyển động theo quỹ đạo
Skeleton và Trajectory có thể riêng rẽ hoặc kết hợp với nhau

Các tệp trong project:
- animated_box.world file: mô phỏng box chuyển động liên tục theo quỹ đạo hình vuông
- walk.world file: mô phỏng con người đi bộ

Định nghĩa quỹ đạo chuyển động bằng tag ```<trajectory>``` có nghĩa là chuyển động theo quỹ đạo định trước mà không liên quan gì tới môi trường (gọi là open-loop trajectory).
Do vậy, còn có thể định nghĩa quỹ đạo bằng plugin. Có một vài plugin có sẵn trong gazebo như libActorPlugin.so:
- Plugin Source code: https://bitbucket.org/osrf/gazebo/raw/default/plugins/ActorPlugin.cc
- Plugin header: https://bitbucket.org/osrf/gazebo/raw/default/plugins/ActorPlugin.hh
