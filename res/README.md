# 系统工作
1. 棋盘落子位置:
 * 获取点击位置(mouse_x,mouse_y)
 * 相对棋盘位置(mouse_x-BOARD_START_X,mouse-BOARD_START_Y)->(mouse_board_x,mouse_board_y)
 * 取整计算最近位置:棋盘坐标位置(round(mouse_board_x/SHIFT_X),round(mouse_board_y/SHIFT_Y))
2. 算杀:
 * 白子为例
 * 遍历棋盘 横，竖，右斜，左斜判断
 * 满足条件退出
3. 基本优化:
   1. 评分差值ok
   2. 搜索深度,棋盘优化处理 ok
   3. 预处理 ok
   4. 算杀，左斜异常. ok
   5. 黑棋胜异常 ok
   
   6. 算法对战
   7. 算法逻辑验证 OK
4. 基本棋力形成,加强棋力算法优化
   1. 当搜索深度加深，搜索时间太慢，动态更改搜索深度(有牺牲的优化:棋力对比)ok
   2. 预处理过程.ok
5. 深度优化
   1. 预处理活二处理 OK
   2. 当前棋子标记 OK
   3. 终局五子5提示，先落子设定.初步下棋 OK
   4. 矩形框优化
   5. 活四空子判断
   6. 平局，结局特效 OK
 # 实力测试:
   1. 先落子预定