# QQR
Approach to QQ recommendation

Approach to QQ(Quiz Question) recommendation
With the development of IT facilities including mobile devices, data storage and computing platform, the digital transformation on education is greatly accelerating in various smart applications, such as intelligent tutoring systems or adaptive learning systems. As a particularly prominent application of smart education, intelligent systems for education is playing a vital role in precision teaching, smart tutoring, and personalized learning. However, we have limited understanding on what is the reality of student engaging with these systems, and what kinds of quiz question (QQ) should be recommended for the engaging students in practical situation. Especially the individual knowledge preference for a certain moment is closely related to personal experience of past learning, as well as temporal scenario with diversity. Therefore, we propose to delineate student engagement trend with learning-action graph and then formalize question recommendation with interactive reinforcement learning. In this study we take individual systems action transition patterns as a temporally evolving action graph, and derive usage patterns in terms of informing future student engagement. Furthermore, we develop a novel framework \textbf {ERLR} (Engagement and Reinforcement Learning based Recommender-Systems) for learning and adapting to students' current preference based on engagement trend and reinforcement learning by collecting interactive data in real time during a learning session. This established recommender framework captures question characters, student dynamic preferences, engagement trend, and that it yields a better learning experience with proper QQ recommendation. Practically we make an earnest endeavor to deploy the proposed ERLR which performs very well in XXXU intelligent learning systems co-developed with YYY Education Group (NYSE: YYY).


一种练习测验卷智能生成模型

问题：

    海量数字化题库资源的积累，为教师教学和学生练习提供了丰富资料，也提出了极大挑战问题，即如何使用海量题库资源的试题自动生成适合学生知识水平的练习测验卷。
    现有研究和实践中，试卷自动生成已被广泛关注，但是存在紧密相关且亟需解决的问题：
        第一个问题是，测验卷题目由教师、系统单方面选择，缺少被试者的参与和反馈，从而缺少对其偏好需求和最近发展区的掌握。
        第二个问题是，测验卷生成后题目无法变动和调整，缺少个性化自适应练习方案。
        第三个问题是，生成的测验卷和学生最近发展区缺少有效匹配，无法起到诊断、巩固和提升的作用。
    因此，迫切需要学生在练习测验时增加互动，反馈个人偏好实际，掌握学生最近发展区阶段，自适应、智能化地实时推荐相符合的测试题目，从而使得练习测验卷起到诊断、巩固和促进学生学习，减轻教师出题负担的作用。
    
实现步骤：动态获取用户的参与度和偏好反馈信息；转换反馈信息为奖励值，更新用户奖励模型；提取奖励模型相应试题特征信息，根据特征信息进行试题搜索，作为生成的下一道题目；调整更新规划策略，向用户推送测验试题，实现练习测验卷智能生成。

预期结果：应用本模型可在与用户交互的基础上智能化、自适应的生成练习测验卷，动态优化调整试题，实现测验卷内容和应试者最近发展区相匹配。

项目特点：

    第一，明提供了第一个基于用户参与度和强化学习技术相结合，实现测验卷智能生成的方法；
    第二，构建了第一个基于学习动作图的用户参与度预测模型即图卷积-长短时记忆网络GCN-LSTM，且效果表现优越；
    第三，所提学习中基于用户参与度和偏好反馈的奖励模型，在交互中实现了测验内容和用户最近发展区的一致；
    第四，所提基于长期奖励价值的规划策略，实现练习测验卷题目情景化、自适应动态调整。
