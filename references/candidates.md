# Candidate Principles

Merge overlapping observations into one entry. Preserve both supporting and contradicting evidence.

## Entry schema

### C-YYYYMMDD-NN — Name

- **Candidate rule**:
- **Scope**:
- **Trigger**:
- **Exceptions**:
- **Source**:
- **Supporting evidence**:
- **Counterevidence**:
- **Proposed activation targets**:
- **Confidence**: low | medium
- **Status**: candidate | trial | confirmed-unrouted
- **Last reviewed**:

### C-20260726-01 — 跨系统探索统一控制面，证据原位

- **Candidate rule**: 当一条不确定探索调用多个既有系统时，只在探索层维护一个轻量的当前检查点；详细进度与证据留在实际产生它的系统，散场时只同步下一入口，不复制过程。
- **Scope**: 同一探索方向跨越学习台账、实践项目与生活记录，需要反复续接的个人工作流。
- **Trigger**: 开始前需要判断“今天去哪个系统、从哪里继续”，或结束后需要在多个系统重复登记同一过程。
- **Exceptions**: 单资源学习可独立使用 Crucible，不必建立轨迹；明确交付仍由 TimeMachine 验收；具有独立生活叙事价值的经历可以另写日记。
- **Source**: tiny-experiments 的有限 PACT 与成长循环；AnleDaily 首条 Agent Memory 轨迹试点。
- **Supporting evidence**: 2026-07-26，Anle 只说“继续 tr260701”，系统即由轨迹检查点路由到 cr260703，完成一组 Agent Memory vs. LLM Memory 辨析后在自然检查点散场；学习判断留在 Crucible，下一入口同步回轨迹，没有要求另写日记。随后 Anle 明确确认 Crucible 仍需支持不挂轨迹的独立分阶段共学，进一步限定了适用范围。
- **Counterevidence**: 目前只有一次短会话证据；尚未验证长时间中断、切换到实践探针或多次往返后是否仍能避免状态漂移。轨迹检查点与底层台账仍各有一句状态摘要，长期维护成本未知。
- **Proposed activation targets**: 尚未评估；若将来确认，应优先检查 [[Trajectories/AGENTS]] 是否已具备自然加载的执行钩子。
- **Confidence**: low
- **Status**: trial
- **Last reviewed**: 2026-07-26

### C-20260726-02 — 证据所有权先于证据问答

- **Candidate rule**: 在协作学习或代码复现中，谁实际执行并观察测试，谁就负责解释测试结果及其证据边界。若要让学习者判断“测试证明了什么／不能证明什么”，必须先让其共同看到足以复核的输入、预期、实际值或差异以及断言链；仅展示测试名、`PASS/FAIL` 或汇总，不得据此反问学习者。
- **Scope**: 助手执行测试、再以测试作为学习检查点、代码 review 依据或掌握度证据的协作场景。
- **Trigger**: 准备把自动测试结果转成对学习者的证据边界问题，或准备声称双方“共同看过”测试证据。
- **Exceptions**: 学习者已经亲自编写或逐行 review 相关断言，并共同观察了足以复核的具体结果；问题发生在测试前，目标是让学习者参与实验设计，而不是事后猜测黑箱结果。
- **Source**: 对 Crucible 全部 14 份可见项目台账及 11 份对应工作台的完整关键词审计；直接证据集中在 cr260702，近邻证据见 cr260705，预防性设计见 cr260706。
- **Supporting evidence**: 直接同类至少出现四个日期。① 2026-07-05，Chase 写完测试后闷头运行、只报结果，Anle 要求“一起跑下看看结果”；当时已约定先摊断言论证点、共同运行、展示输出。② 2026-07-17，Chase 再次后台运行 RoPE 测试，只报 `16 passed`，随即要求 Anle 判断证据边界；Anle 直接指出“都没让我看过测试的结果，这怎么回答”。③ 2026-07-20，Chase 把完整输出留在工具区，纠正后又只展示逐项 `PASSED`；Anle 先追问“测试结果在哪”，随后指出测试名称仍不能呈现输入、预期、实际结果与断言链，证据边界 gate 被永久取消。④ 2026-07-26，Chase 只展示梯度累积单测 `PASSED` 与汇总，又追问测试能证明／不能证明什么；Anle 指出自己看不到详细内容，该提问没有意义且属于形式主义。近邻机制在 cr260705 又出现三次：Chase 自己把代码写完、只给结果，Anle 要求参与书写本身；这支持更底层的共同原因——助手独占过程后，结果交付不能替代学习者的观察与参与。cr260706 已把“先看实验要验证什么、实际运行、一起看结果和限制”写入活动规则，但尚无完成记录可作成功证据。
- **Counterevidence**: cr260603、cr260608 等台账存在 runner／测试通过及“证明／不证明什么”的总结，但台账摘要不足以确认 Anle 当时是否共同观察了具体证据，沉默不能视作反证。尚未观察到一次严格按本候选规则展示输入、预期、实际值或差异与断言链后，再由学习者自愿进行证据边界判断的成功案例；也未验证学习者亲自设计断言时所需的最低展示粒度。
- **Proposed activation targets**: `D:\Subspace\ObsidianDB\AnleDaily\Crucible\AGENTS.md`，在所有 Crucible 学习与复现任务开始前自然加载；写入前仍需 Anle 对该目标明确授权。
- **Confidence**: medium
- **Status**: candidate
- **Last reviewed**: 2026-07-26
