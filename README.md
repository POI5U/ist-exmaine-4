# 姿态解算代码: 
## 采用卡尔曼滤波
## 一个init对应一个角度的滤波

# 例程:
## 硬件使用 stm32f103c8t6 + mpu6050 + OLED(6线spi)
## 软件使用 标准库 + FreeRTOS + 6轴卡尔曼滤波算法解算(pitch + roll)角度
## yaw直接通过积分获取(会出现漂移)
双任务( MPU6050解算 和 OLED显示输出 )
mpu6050 连接 stm32f103c8t6 的 iic2


