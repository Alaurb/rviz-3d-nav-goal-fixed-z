# rviz-3d-nav-goal-fixed-z

只需把这两个文件覆盖到你的 rviz_plugins 包里， `catkin_make`后重新运行示例，使用3D Nav Goal选择目标点即可规划路径。
也可点击rviz左上角**Panels**选择 **Tool Properties** 在**3D Nav Goal**里看到 **Default Z** 输入框，根据情况修改为不为0的数。

## Usage
1. 备份原 `goal_tool.h` / `goal_tool.cpp`
2. 用本仓库两个文件替换
3. `catkin_make && source devel/setup.bash`
4. `rviz` → **Panels** → **Tool Properties**→ **Goal3DTool** → 设置 **Default Z** → 完成
