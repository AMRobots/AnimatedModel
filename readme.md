Tạo model chuyển động trong gazebo, theo ví dụ:
http://gazebosim.org/tutorials?tut=actor&cat=build_robot#Scriptedtrajectories

Mô hình chuyển động gồm:
- Skeleton: các link trong model chuyển động với nhau. ví dụ tay, chân,...
- Trajectory: toàn bộ model chuyển động theo quỹ đạo
Skeleton và Trajectory có thể riêng rẽ hoặc kết hợp với nhau

Các tệp trong project:
- animated_box.world file: mô phỏng box chuyển động liên tục theo quỹ đạo hình vuông
- walk.world file: mô phỏng con người đi bộ
