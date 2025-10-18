# rviz-3d-nav-goal-fixed-z
https://github.com/ZJU-FAST-Lab/3D2M-planner.git
针对工程直接运行例程无法规划路径的修补。
覆盖原工程rviz_plugins包中的同名文件， `catkin_make`后重新运行示例，使用3D Nav Goal选择目标点即可规划路径。
后续可点击rviz左上角**Panels**选择 **Tool Properties** ，在**3D Nav Goal**里看到 **Default Z** 输入框，根据情况修改z值。

## Usage
1. 备份原 `goal_tool.h` / `goal_tool.cpp`
2. 用本仓库两个文件替换
3. `catkin_make && source devel/setup.bash`
4. `rviz` → **Panels** → **Tool Properties**→ **Goal3DTool** → 设置 **Default Z** → 完成
