# Config Reference ภาษาไทย

สารบัญคีย์ทั้งหมดจาก control/config.txt ของ OpenKore branch master พร้อมคำอธิบายไทยแบบย่อ

> อัปเดตจาก OpenKore master เมื่อ 2026-08-10 — ห้ามใส่รหัสผ่านจริงในไฟล์ตัวอย่างหรือเผยแพร่ใน Repository

พบทั้งหมด **605 คีย์/รายการ**

## วิธีอ่าน

- `0` มักหมายถึงปิด และ `1` มักหมายถึงเปิด แต่ให้ยึดคำอธิบายของคีย์นั้นเป็นหลัก
- ค่า Template เป็นค่าจากไฟล์ต้นฉบับ ไม่ใช่ค่าที่เหมาะกับทุกเซิร์ฟเวอร์
- `password` และ `loginPinCode` ต้องเก็บเป็นความลับ

## Debug และ Plugins

| คีย์ | หน้าที่โดยสรุป | ชนิดค่า | ค่าใน Template |
|---|---|---|---|
| `debug` | ตัวเลือกสำหรับตรวจสอบระบบหรือ Plugins | ตัวเลข | 0 |
| `debugAssertOnNetwork` | ตัวเลือกสำหรับตรวจสอบระบบหรือ Plugins | ตัวเลข | 0 |
| `debugPacket_unparsed` | ตัวเลือกสำหรับตรวจสอบระบบหรือ Plugins | ตัวเลข | 0 |
| `debugPacket_received` | ตัวเลือกสำหรับตรวจสอบระบบหรือ Plugins | ตัวเลข | 0 |
| `debugPacket_ro_received` | ตัวเลือกสำหรับตรวจสอบระบบหรือ Plugins | ตัวเลข | 0 |
| `debugPacket_ro_sent` | ตัวเลือกสำหรับตรวจสอบระบบหรือ Plugins | ตัวเลข | 0 |
| `debugPacket_sent` | ตัวเลือกสำหรับตรวจสอบระบบหรือ Plugins | ตัวเลข | 0 |
| `debugPacket_exclude` | ตัวเลือกสำหรับตรวจสอบระบบหรือ Plugins | ค่าเปล่า/ข้อความ | (ว่าง) |
| `debugPacket_include` | ตัวเลือกสำหรับตรวจสอบระบบหรือ Plugins | ค่าเปล่า/ข้อความ | (ว่าง) |
| `debugPacket_include_dumpMethod` | ตัวเลือกสำหรับตรวจสอบระบบหรือ Plugins | ค่าเปล่า/ข้อความ | (ว่าง) |
| `debugDomains` | ตัวเลือกสำหรับตรวจสอบระบบหรือ Plugins | ค่าเปล่า/ข้อความ | (ว่าง) |
| `eventMacro_orphans` | ตัวเลือกสำหรับตรวจสอบระบบหรือ Plugins | ข้อความหรือรายการ | terminate |
| `eventMacro_CheckOnAI` | ตัวเลือกสำหรับตรวจสอบระบบหรือ Plugins | ข้อความหรือรายการ | auto |
| `eventMacro_notWhenInQueue` | ตัวเลือกสำหรับตรวจสอบระบบหรือ Plugins | ข้อความหรือรายการ | storageAuto, buyAuto, sellAuto |
| `eventMacro_file` | ตัวเลือกสำหรับตรวจสอบระบบหรือ Plugins | ข้อความหรือรายการ | eventMacros.txt |
| `avoidObstacles_enable_move` | ตัวเลือกสำหรับตรวจสอบระบบหรือ Plugins | ตัวเลข | 1 |
| `avoidObstacles_enable_remove` | ตัวเลือกสำหรับตรวจสอบระบบหรือ Plugins | ตัวเลข | 1 |
| `avoidObstacles_enable_avoid_portals` | ตัวเลือกสำหรับตรวจสอบระบบหรือ Plugins | ตัวเลข | 1 |
| `avoidObstacles_adjust_route_step` | ตัวเลือกสำหรับตรวจสอบระบบหรือ Plugins | ตัวเลข | 1 |
| `avoidObstacles_weight_limit` | ตัวเลือกสำหรับตรวจสอบระบบหรือ Plugins | ตัวเลข | 65000 |

## Homunculus Mercenary และ Pet

| คีย์ | หน้าที่โดยสรุป | ชนิดค่า | ค่าใน Template |
|---|---|---|---|
| `mercenary_attackAuto` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 2 |
| `mercenary_attackAuto_routeToLock` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `mercenary_attackAuto_outOfLock` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `mercenary_attackAuto_party` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `mercenary_attackAuto_notInTown` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `mercenary_attackAuto_notWhile_storageAuto` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `mercenary_attackAuto_notWhile_buyAuto` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `mercenary_attackAuto_notWhile_sellAuto` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `mercenary_attackAuto_considerDamagedAggressive` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_attackAuto_considerAggressiveIfCastOnCastSensor` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_attackAuto_onlyWhenSafe` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_attackAuto_duringRandomWalk` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_attackAuto_duringItemsTake` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_attackDistance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `mercenary_attackMaxDistance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `mercenary_attackDistanceAuto` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `mercenary_attackMaxRouteTime` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 4 |
| `mercenary_attackCanSnipe` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_attackCheckLOS` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `mercenary_attackRouteMaxPathDistance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 20 |
| `mercenary_attackUseWeapon` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `mercenary_attackNoGiveup` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_attackChangeTarget` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `mercenary_attack_dance_melee` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_attack_dance_ranged` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_attackBeyondMaxDistance_waitForAgressive` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `mercenary_attackBeyondMaxDistance_sendAttackWhileWaiting` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_attackSendAttackWithMove` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_attackWaitApproachFinish` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `mercenary_route_rescueWhenLost` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_route_stopDuringAttack` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_route_waitMinDistance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 10 |
| `mercenary_runFromTarget` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_runFromTarget_inAdvance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_runFromTarget_dist` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 5 |
| `mercenary_runFromTarget_minStep` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 7 |
| `mercenary_runFromTarget_maxPathDistance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 20 |
| `mercenary_runFromTarget_noAttackMethodFallback` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_runFromTarget_noAttackMethodFallback_attackMaxDist` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 14 |
| `mercenary_runFromTarget_noAttackMethodFallback_minStep` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 8 |
| `mercenary_idleWalkType` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `mercenary_followMode` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `mercenary_followDistanceMin` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 3 |
| `mercenary_followDistanceMax` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 10 |
| `mercenary_moveNearWhenIdle` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `mercenary_moveNearWhenIdle_minDistance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 3 |
| `mercenary_moveNearWhenIdle_maxDistance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 8 |
| `mercenary_route_step` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 10 |
| `mercenary_tankMode` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_tankModeTarget` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `mercenary_teleportAuto_hp` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 10 |
| `mercenary_teleportAuto_maxDmg` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 500 |
| `mercenary_teleportAuto_maxDmgInLock` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_teleportAuto_deadly` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `mercenary_teleportAuto_unstuck` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_teleportAuto_dropTarget` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_teleportAuto_dropTargetEngaged` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `mercenary_teleportAuto_dropTargetKS` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_teleportAuto_totalDmg` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_teleportAuto_totalDmgInLock` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `mercenary_teleportAuto_attackedWhenSitting` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_attackAuto` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 2 |
| `homunculus_attackAuto_routeToLock` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_attackAuto_outOfLock` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_attackAuto_party` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_attackAuto_notInTown` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_attackAuto_notWhile_storageAuto` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_attackAuto_notWhile_buyAuto` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_attackAuto_notWhile_sellAuto` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_attackAuto_considerDamagedAggressive` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_attackAuto_considerAggressiveIfCastOnCastSensor` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_attackAuto_onlyWhenSafe` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_attackAuto_duringRandomWalk` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_attackAuto_duringItemsTake` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_attackDistance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_attackMaxDistance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_attackDistanceAuto` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_attackMaxRouteTime` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 4 |
| `homunculus_attackCanSnipe` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_attackCheckLOS` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_attackRouteMaxPathDistance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 20 |
| `homunculus_attackUseWeapon` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_attackNoGiveup` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_attackChangeTarget` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_attack_dance_melee` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_attackBeyondMaxDistance_waitForAgressive` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_attackBeyondMaxDistance_sendAttackWhileWaiting` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_attackSendAttackWithMove` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_attackWaitApproachFinish` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_route_rescueWhenLost` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_route_stopDuringAttack` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_route_waitMinDistance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_runFromTarget` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_runFromTarget_dist` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 5 |
| `homunculus_runFromTarget_minStep` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 7 |
| `homunculus_runFromTarget_maxPathDistance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 20 |
| `homunculus_runFromTarget_noAttackMethodFallback` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_runFromTarget_noAttackMethodFallback_attackMaxDist` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 14 |
| `homunculus_runFromTarget_noAttackMethodFallback_minStep` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 8 |
| `homunculus_idleWalkType` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_followMode` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_followDistanceMin` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 3 |
| `homunculus_followDistanceMax` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 10 |
| `homunculus_moveNearWhenIdle` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_moveNearWhenIdle_minDistance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 3 |
| `homunculus_moveNearWhenIdle_maxDistance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 8 |
| `homunculus_route_step` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 10 |
| `homunculus_tankMode` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_tankModeTarget` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `homunculus_StandByAuto` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_teleportAuto_hp` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 10 |
| `homunculus_teleportAuto_maxDmg` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 500 |
| `homunculus_teleportAuto_maxDmgInLock` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_teleportAuto_deadly` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_teleportAuto_unstuck` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_teleportAuto_dropTarget` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_teleportAuto_dropTargetEngaged` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_teleportAuto_dropTargetKS` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_teleportAuto_totalDmg` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_teleportAuto_totalDmgInLock` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_teleportAuto_attackedWhenSitting` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `homunculus_autoFeed` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `homunculus_hunger` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 15 |
| `homunculus_return` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 11 |
| `homunculus_autoFeedAllowedMaps` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `pet_autoFeed` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `pet_hunger` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 25 |
| `pet_return` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 20 |

## Teleport และความปลอดภัย

| คีย์ | หน้าที่โดยสรุป | ชนิดค่า | ค่าใน Template |
|---|---|---|---|
| `teleportAuto_hp` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 10 |
| `teleportAuto_sp` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 0 |
| `teleportAuto_idle` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 0 |
| `teleportAuto_portal` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 0 |
| `teleportAuto_search` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 0 |
| `teleportAuto_minAggressives` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 0 |
| `teleportAuto_minAggressivesInLock` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 0 |
| `teleportAuto_onlyWhenSafe` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 0 |
| `teleportAuto_maxDmg` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 500 |
| `teleportAuto_maxDmgInLock` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 0 |
| `teleportAuto_deadly` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 1 |
| `teleportAuto_useSkill` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 1 |
| `teleportAuto_useChatCommand` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ค่าเปล่า/ข้อความ | (ว่าง) |
| `teleportAuto_allPlayers` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 0 |
| `teleportAuto_notPlayers` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ค่าเปล่า/ข้อความ | (ว่าง) |
| `teleportAuto_atkCount` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 0 |
| `teleportAuto_atkMiss` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 10 |
| `teleportAuto_unstuck` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 0 |
| `teleportAuto_lostTarget` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 0 |
| `teleportAuto_dropTarget` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 0 |
| `teleportAuto_dropTargetEngaged` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 1 |
| `teleportAuto_dropTargetKS` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 0 |
| `teleportAuto_dropTargetHidden` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 0 |
| `teleportAuto_attackedWhenSitting` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 0 |
| `teleportAuto_totalDmg` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 0 |
| `teleportAuto_totalDmgInLock` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ตัวเลข | 0 |
| `teleportAuto_equip_leftAccessory` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ค่าเปล่า/ข้อความ | (ว่าง) |
| `teleportAuto_equip_rightAccessory` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ค่าเปล่า/ข้อความ | (ว่าง) |
| `teleportAuto_lostHomunculus` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ค่าเปล่า/ข้อความ | (ว่าง) |
| `teleportAuto_useItemForRespawn` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ค่าเปล่า/ข้อความ | (ว่าง) |
| `teleportAuto_item1` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ค่าเปล่า/ข้อความ | (ว่าง) |
| `teleportAuto_item2` | กำหนดเงื่อนไขและวิธีใช้ Teleport | ค่าเปล่า/ข้อความ | (ว่าง) |

## แผนที่และเส้นทาง

| คีย์ | หน้าที่โดยสรุป | ชนิดค่า | ค่าใน Template |
|---|---|---|---|
| `clientSight` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 17 |
| `lockMap` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ค่าเปล่า/ข้อความ | (ว่าง) |
| `lockMap_x` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ค่าเปล่า/ข้อความ | (ว่าง) |
| `lockMap_y` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ค่าเปล่า/ข้อความ | (ว่าง) |
| `lockMap_randX` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ค่าเปล่า/ข้อความ | (ว่าง) |
| `lockMap_randY` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ค่าเปล่า/ข้อความ | (ว่าง) |
| `route_escape_reachedNoPortal` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 1 |
| `route_escape_randomWalk` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 1 |
| `route_escape_shout` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ค่าเปล่า/ข้อความ | (ว่าง) |
| `route_randomWalk` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 1 |
| `route_randomWalk_inLockOnly` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 0 |
| `route_randomWalk_inTown` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 0 |
| `route_randomWalk_maxRouteTime` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 75 |
| `route_maxWarpFee` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ค่าเปล่า/ข้อความ | (ว่าง) |
| `route_maxNpcTries` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 5 |
| `route_teleport` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 0 |
| `route_teleport_minDistance` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 75 |
| `route_teleport_maxTries` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 8 |
| `route_teleport_notInMaps` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ค่าเปล่า/ข้อความ | (ว่าง) |
| `route_warpByItem` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 0 |
| `route_warpByItem_chaining` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 0 |
| `route_warpByItem_minDistance` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 150 |
| `route_warpItem_minGain` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 0 |
| `route_warpItem_routeCostHeuristic_max` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 10000 |
| `route_warpItem_routeCostProbe_maxPerTick` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 6 |
| `route_warpItem_routeCostCache_max` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 3000 |
| `route_step` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 10 |
| `route_removeMissingPortals_NPC` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 1 |
| `route_removeMissingPortals` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 0 |
| `route_tryToGuessMissingPortalByDistance` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 1 |
| `route_reAddMissingPortals` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 1 |
| `route_avoidWalls` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 1 |
| `route_randomFactor` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 0 |
| `EdenPortalExit` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `maxUnobstructedWalkPathDistance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 17 |
| `maxObstructedWalkPathDistance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 14 |
| `runFromTarget` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 0 |
| `runFromTarget_inAdvance` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 0 |
| `runFromTarget_dist` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 5 |
| `runFromTarget_minStep` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 7 |
| `runFromTarget_maxPathDistance` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 13 |
| `runFromTarget_noAttackMethodFallback` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 0 |
| `runFromTarget_noAttackMethodFallback_attackMaxDist` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 14 |
| `runFromTarget_noAttackMethodFallback_minStep` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 8 |
| `saveMap` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ค่าเปล่า/ข้อความ | (ว่าง) |
| `saveMap_x` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ค่าเปล่า/ข้อความ | (ว่าง) |
| `saveMap_y` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ค่าเปล่า/ข้อความ | (ว่าง) |
| `saveMap_warp` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 0 |
| `saveMap_warpToBuyOrSell` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ตัวเลข | 1 |
| `saveMap_warp_minDistance` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ค่าเปล่า/ข้อความ | (ว่าง) |
| `saveMap_warpChatCommand` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ค่าเปล่า/ข้อความ | (ว่าง) |
| `memo1` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ค่าเปล่า/ข้อความ | (ว่าง) |
| `memo2` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ค่าเปล่า/ข้อความ | (ว่าง) |
| `memo3` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ค่าเปล่า/ข้อความ | (ว่าง) |
| `memo4` | กำหนดการเดินทาง แผนที่ปลอดภัย และการหลบเป้าหมาย | ค่าเปล่า/ข้อความ | (ว่าง) |

## ไอเทม NPC และคลัง

| คีย์ | หน้าที่โดยสรุป | ชนิดค่า | ค่าใน Template |
|---|---|---|---|
| `itemsTakeAuto` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 2 |
| `itemsTakeAuto_party` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 0 |
| `itemsGatherAuto` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 2 |
| `itemsGatherAuto_notInTown` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 0 |
| `itemsGatherAutoMinPlayerDistance` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 6 |
| `itemsGatherAutoMinPortalDistance` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 5 |
| `itemsMaxWeight` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 89 |
| `itemsMaxWeight_sellOrStore` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 48 |
| `itemsMaxNum_sellOrStore` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 99 |
| `cartMaxWeight` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 7900 |
| `itemsTakeGreed` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 0 |
| `itemsCheckWeight` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 1 |
| `shopAuto_open` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 0 |
| `buyerShopAuto_open` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 0 |
| `dealAuto` | กำหนดพฤติกรรมร่วมกับผู้เล่นหรือปาร์ตี้ | ตัวเลข | 1 |
| `dealAuto_names` | กำหนดพฤติกรรมร่วมกับผู้เล่นหรือปาร์ตี้ | ค่าเปล่า/ข้อความ | (ว่าง) |
| `dealMaxItems` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 10 |
| `repairAuto` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 0 |
| `repairAuto_list` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `repairAuto_npc` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `repairAuto_standpoint` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `repairAuto_distance` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 3 |
| `repairAuto_maxDistance` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `repairAuto_npc_steps` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ข้อความหรือรายการ | c r0 c c r0 n |
| `repairAuto_useSkill` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 0 |
| `repairAuto_equipAfter` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 1 |
| `repairAuto_warp` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 0 |
| `repairAuto_inTownOnly` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 0 |
| `useSelf_skill_smartHeal` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `autoSwitch_default_rightHand` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `autoSwitch_default_leftHand` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `autoSwitch_default_arrow` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `sellAuto` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 0 |
| `sellAuto_npc` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `sellAuto_standpoint` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `sellAuto_distance` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 3 |
| `sellAuto_maxDistance` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `sellAuto_npc_steps` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ข้อความหรือรายการ | s |
| `storageAuto` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 0 |
| `storageAuto_onStart` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 0 |
| `storageAuto_npc` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `storageAuto_standpoint` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `storageAuto_distance` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 3 |
| `storageAuto_maxDistance` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `storageAuto_npc_type` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 1 |
| `storageAuto_type` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 0 |
| `storageAuto_npc_steps` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `storageAuto_password` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `storageAuto_keepOpen` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 0 |
| `storageAuto_useChatCommand` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `storageAuto_useItem` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ตัวเลข | 0 |
| `storageAuto_useItem_item` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `storageAuto_notAfterDeath` | กำหนดการจัดการไอเทม น้ำหนัก NPC หรือคลัง | ค่าเปล่า/ข้อความ | (ว่าง) |

## การเชื่อมต่อและ XKore

| คีย์ | หน้าที่โดยสรุป | ชนิดค่า | ค่าใน Template |
|---|---|---|---|
| `poseidonServer` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ข้อความหรือรายการ | 127.0.0.1 |
| `poseidonPort` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 24390 |
| `poseidonTimeout` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 5 |
| `bindIp` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `forceMapIP` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `XKore` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `XKore_port` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 2350 |
| `XKore_dll` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ข้อความหรือรายการ | NetRedirect.dll |
| `XKore_injectDLL` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `XKore_autoAttachIfOneExe` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `XKore_silent` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `XKore_lookForProcess` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `XKore_bypassBotDetection` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `XKore_exeName` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ข้อความหรือรายการ | ragexe.exe |
| `XKore_listenIp` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ข้อความหรือรายการ | 127.0.0.1 |
| `XKore_listenPort` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 6901 |
| `XKore_listenPort_map` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `XKore_listenPort_char` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `XKore_publicIp` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ข้อความหรือรายการ | 127.0.0.1 |
| `XKore_ID` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `secureAdminPassword` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `adminPassword` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `callSign` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `commandPrefix` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ข้อความหรือรายการ | ; |
| `callSignGM` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `inGameAuth` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `macAddress` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `pauseCharLogin` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 2 |
| `pauseCharServer` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `pauseMapServer` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `ignoreInvalidLogin` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `whenInGame_requestCashPoints` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `message_length_max` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 80 |

## การต่อสู้และเป้าหมาย

| คีย์ | หน้าที่โดยสรุป | ชนิดค่า | ค่าใน Template |
|---|---|---|---|
| `attackAuto` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 2 |
| `attackAuto_routeToLock` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 1 |
| `attackAuto_outOfLock` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 1 |
| `attackAuto_party` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 1 |
| `attackAuto_onlyWhenSafe` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 0 |
| `attackAuto_followTarget` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 1 |
| `attackAuto_notInTown` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 1 |
| `attackAuto_notWhile_storageAuto` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 1 |
| `attackAuto_notWhile_buyAuto` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 1 |
| `attackAuto_notWhile_sellAuto` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 1 |
| `attackAuto_considerDamagedAggressive` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 0 |
| `attackAuto_considerAggressiveIfCastOnCastSensor` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 0 |
| `attackAllowStartStorageBuySell` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 1 |
| `attackDistance` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 1 |
| `attackDistanceAuto` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 1 |
| `attackMaxDistance` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 1 |
| `attackMaxRouteTime` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 4 |
| `attackMinPlayerDistance` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 2 |
| `attackMinPortalDistance` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 4 |
| `attackUseWeapon` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 1 |
| `attackNoGiveup` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 0 |
| `attackCanSnipe` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 0 |
| `attackCheckLOS` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 1 |
| `attackRouteMaxPathDistance` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 20 |
| `attackLooters` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 0 |
| `attackLooters_dist` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 1 |
| `attackChangeTarget` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 1 |
| `aggressiveAntiKS` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `attackUpdateMonsterPos` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 1 |
| `attackBeyondMaxDistance_waitForAgressive` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 0 |
| `attackBeyondMaxDistance_sendAttackWhileWaiting` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 0 |
| `attackSendAttackWithMove` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 0 |
| `attackWaitApproachFinish` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ตัวเลข | 1 |
| `autoMoveOnDeath` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `autoMoveOnDeath_x` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `autoMoveOnDeath_y` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `autoMoveOnDeath_map` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `attackEquip_topHead` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ค่าเปล่า/ข้อความ | (ว่าง) |
| `attackEquip_midHead` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ค่าเปล่า/ข้อความ | (ว่าง) |
| `attackEquip_lowHead` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ค่าเปล่า/ข้อความ | (ว่าง) |
| `attackEquip_leftHand` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ค่าเปล่า/ข้อความ | (ว่าง) |
| `attackEquip_rightHand` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ค่าเปล่า/ข้อความ | (ว่าง) |
| `attackEquip_leftAccessory` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ค่าเปล่า/ข้อความ | (ว่าง) |
| `attackEquip_rightAccessory` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ค่าเปล่า/ข้อความ | (ว่าง) |
| `attackEquip_robe` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ค่าเปล่า/ข้อความ | (ว่าง) |
| `attackEquip_armor` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ค่าเปล่า/ข้อความ | (ว่าง) |
| `attackEquip_shoes` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ค่าเปล่า/ข้อความ | (ว่าง) |
| `attackEquip_arrow` | ควบคุมระยะ วิธี และเงื่อนไขการโจมตี | ค่าเปล่า/ข้อความ | (ว่าง) |

## การตั้งค่าอื่น ๆ

| คีย์ | หน้าที่โดยสรุป | ชนิดค่า | ค่าใน Template |
|---|---|---|---|
| `alias_heal` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ข้อความหรือรายการ | sp 28 |
| `allowedMaps` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `allowedMaps_reaction` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `startTime` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `stopTime` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `minTime` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `varTime` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `lvl` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `joblvl` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `autoMakeArrows` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `autoRestart` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `autoRestartMin` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 10800 |
| `autoRestartSeed` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 3600 |
| `autoRestartSleep` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `autoSleepMin` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 900 |
| `autoSleepSeed` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 900 |
| `autoResponse` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `autoResponseOnHeal` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `autoSpell` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `autoSpell_safe` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `autoPoison` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `avoidGM_namePattern` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `avoidGM_near` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `avoidGM_near_inTown` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `avoidGM_talk` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `avoidGM_reconnect` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1800 |
| `avoidGM_ignoreList` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `avoidList` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `avoidList_inLockOnly` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `avoidList_reconnect` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1800 |
| `avoidList_ignoreList` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `avoidHiddenActors` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `avoidHiddenMonsters` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `cachePlayerNames` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `cachePlayerNames_duration` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 900 |
| `cachePlayerNames_maxSize` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 100 |
| `dcPause` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `dcOnDeath` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `dcOnDualLogin` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `dcOnDisconnect` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `dcOnEmptyArrow` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `dcOnMaxReconnections` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `dcOnMute` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `dcOnPM` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `dcOnZeny` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `dcOnStorageFull` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `dcOnPlayer` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `dcOnServerShutDown` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `dcOnServerClose` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `dcOnJobLevel` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `dcOnLevel` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `shop_random` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `shop_useSkill` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `buyerShop_random` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `githubURL` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `githubIssueURL` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `manualURL` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ข้อความหรือรายการ | https://openkore.com/wiki/Manual |
| `forumURL` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ข้อความหรือรายการ | https://forums.openkore.com |
| `autoTalkCont` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `noAutoSkill` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `missDamage` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `tankersList` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `status_mapProperty` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `status_mapType` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `monster_filter` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `lvl` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `dist` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `maxDist` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `maxCastTime` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `minCastTime` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `previousDamage` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `monsters` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `notMonsters` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `maxAttempts` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `maxUses` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `isSelfSkill` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `isStartSkill` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `equip_topHead` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `equip_midHead` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `equip_lowHead` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `equip_leftHand` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `equip_rightHand` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `equip_leftAccessory` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `equip_rightAccessory` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `equip_robe` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `equip_armor` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `equip_shoes` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `equip_arrow` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `afterSkill` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `waitBeforeUse` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `autoCombo` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `smartEncore` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `noSmartHeal` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `partySkillDistance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ข้อความหรือรายการ | 0..8 |
| `target` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `notPartyOnly` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `rightHand` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `leftHand` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `arrow` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `distance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `useWeapon` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `topHead` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `midHead` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `lowHead` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `leftAccessory` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `rightAccessory` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `robe` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `armor` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `shoes` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `weight` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `whileSitting` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `dcOnEmpty` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `npc` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `npc_steps` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ข้อความหรือรายการ | b |
| `isMarket` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `standpoint` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `distance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 3 |
| `price` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `minAmount` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 2 |
| `maxAmount` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 3 |
| `batchSize` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `onlyIdentified` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `zeny` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `minDistance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `maxDistance` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `dcOnEmpty` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `rodexMaxItems` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 5 |
| `relogAfterStorage` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `minStorageZeny` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 50 |
| `npcWrongStepsMethod` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `passive` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `history_max` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 50 |
| `enabled` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `penalty_dist` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ข้อความหรือรายการ | 1000, 1000, 1000, 20 |
| `danger_dist` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ข้อความหรือรายการ | 10, 10, 10, 1 |
| `prohibited_dist` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 2 |
| `drop_target_when_near_dist` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 3 |
| `drop_destination_when_near_dist` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 3 |

## ตัวละคร ปาร์ตี้ และผู้ช่วย

| คีย์ | หน้าที่โดยสรุป | ชนิดค่า | ค่าใน Template |
|---|---|---|---|
| `follow` | กำหนดพฤติกรรมร่วมกับผู้เล่นหรือปาร์ตี้ | ตัวเลข | 0 |
| `followTarget` | กำหนดพฤติกรรมร่วมกับผู้เล่นหรือปาร์ตี้ | ค่าเปล่า/ข้อความ | (ว่าง) |
| `followEmotion` | กำหนดพฤติกรรมร่วมกับผู้เล่นหรือปาร์ตี้ | ตัวเลข | 1 |
| `followEmotion_distance` | กำหนดพฤติกรรมร่วมกับผู้เล่นหรือปาร์ตี้ | ตัวเลข | 4 |
| `followFaceDirection` | กำหนดพฤติกรรมร่วมกับผู้เล่นหรือปาร์ตี้ | ตัวเลข | 0 |
| `followDistanceMax` | กำหนดพฤติกรรมร่วมกับผู้เล่นหรือปาร์ตี้ | ตัวเลข | 6 |
| `followDistanceMin` | กำหนดพฤติกรรมร่วมกับผู้เล่นหรือปาร์ตี้ | ตัวเลข | 3 |
| `followLostStep` | กำหนดพฤติกรรมร่วมกับผู้เล่นหรือปาร์ตี้ | ตัวเลข | 12 |
| `followSitAuto` | กำหนดพฤติกรรมร่วมกับผู้เล่นหรือปาร์ตี้ | ตัวเลข | 0 |
| `followBot` | กำหนดพฤติกรรมร่วมกับผู้เล่นหรือปาร์ตี้ | ตัวเลข | 0 |
| `sitAuto_hp_lower` | กำหนดเงื่อนไขนั่งพักตาม HP/SP หรือสถานะ | ตัวเลข | 40 |
| `sitAuto_hp_upper` | กำหนดเงื่อนไขนั่งพักตาม HP/SP หรือสถานะ | ตัวเลข | 100 |
| `sitAuto_sp_lower` | กำหนดเงื่อนไขนั่งพักตาม HP/SP หรือสถานะ | ตัวเลข | 0 |
| `sitAuto_sp_upper` | กำหนดเงื่อนไขนั่งพักตาม HP/SP หรือสถานะ | ตัวเลข | 0 |
| `sitAuto_follow` | กำหนดเงื่อนไขนั่งพักตาม HP/SP หรือสถานะ | ตัวเลข | 0 |
| `sitAuto_over_50` | กำหนดเงื่อนไขนั่งพักตาม HP/SP หรือสถานะ | ตัวเลข | 0 |
| `sitAuto_idle` | กำหนดเงื่อนไขนั่งพักตาม HP/SP หรือสถานะ | ตัวเลข | 1 |
| `sitAuto_look` | กำหนดเงื่อนไขนั่งพักตาม HP/SP หรือสถานะ | ค่าเปล่า/ข้อความ | (ว่าง) |
| `sitAuto_look_from_wall` | กำหนดเงื่อนไขนั่งพักตาม HP/SP หรือสถานะ | ค่าเปล่า/ข้อความ | (ว่าง) |
| `sitAuto_look_delay` | กำหนดเงื่อนไขนั่งพักตาม HP/SP หรือสถานะ | ค่าเปล่า/ข้อความ | (ว่าง) |
| `sitTensionRelax` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `statsAddAuto` | เปิดการเพิ่มค่าสถานะหรือสกิลอัตโนมัติ | ตัวเลข | 0 |
| `statsAddAuto_list` | เปิดการเพิ่มค่าสถานะหรือสกิลอัตโนมัติ | ค่าเปล่า/ข้อความ | (ว่าง) |
| `statsAddAuto_dontUseBonus` | เปิดการเพิ่มค่าสถานะหรือสกิลอัตโนมัติ | ตัวเลข | 0 |
| `statsAdd_over_99` | เปิดการเพิ่มค่าสถานะหรือสกิลอัตโนมัติ | ตัวเลข | 1 |
| `skillsAddAuto` | เปิดการเพิ่มค่าสถานะหรือสกิลอัตโนมัติ | ตัวเลข | 0 |
| `skillsAddAuto_list` | เปิดการเพิ่มค่าสถานะหรือสกิลอัตโนมัติ | ค่าเปล่า/ข้อความ | (ว่าง) |
| `tankMode` | กำหนดพฤติกรรมร่วมกับผู้เล่นหรือปาร์ตี้ | ตัวเลข | 0 |
| `tankModeTarget` | กำหนดพฤติกรรมร่วมกับผู้เล่นหรือปาร์ตี้ | ค่าเปล่า/ข้อความ | (ว่าง) |
| `partyAuto` | กำหนดพฤติกรรมร่วมกับผู้เล่นหรือปาร์ตี้ | ตัวเลข | 1 |
| `partyAutoShare` | กำหนดพฤติกรรมร่วมกับผู้เล่นหรือปาร์ตี้ | ตัวเลข | 0 |
| `partyAutoShareItem` | กำหนดพฤติกรรมร่วมกับผู้เล่นหรือปาร์ตี้ | ตัวเลข | 0 |
| `partyAutoShareItemDiv` | กำหนดพฤติกรรมร่วมกับผู้เล่นหรือปาร์ตี้ | ตัวเลข | 0 |
| `guildAutoDeny` | กำหนดพฤติกรรมร่วมกับผู้เล่นหรือปาร์ตี้ | ตัวเลข | 1 |
| `attendanceAuto` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |

## บัญชีและเซิร์ฟเวอร์

| คีย์ | หน้าที่โดยสรุป | ชนิดค่า | ค่าใน Template |
|---|---|---|---|
| `master` | ข้อมูลเลือกเซิร์ฟเวอร์และตัวละคร | ค่าเปล่า/ข้อความ | (ว่าง) |
| `server` | ข้อมูลเลือกเซิร์ฟเวอร์และตัวละคร | ค่าเปล่า/ข้อความ | (ว่าง) |
| `username` | ข้อมูลเลือกเซิร์ฟเวอร์และตัวละคร | ค่าเปล่า/ข้อความ | (ว่าง) |
| `password` | ข้อมูลเลือกเซิร์ฟเวอร์และตัวละคร | ค่าเปล่า/ข้อความ | (ว่าง) |
| `loginPinCode` | ควบคุมการแสดงผล หน้าต่าง และ Log | ค่าเปล่า/ข้อความ | (ว่าง) |
| `char` | ข้อมูลเลือกเซิร์ฟเวอร์และตัวละคร | ค่าเปล่า/ข้อความ | (ว่าง) |
| `otpSeed` | ข้อมูลเลือกเซิร์ฟเวอร์และตัวละคร | ค่าเปล่า/ข้อความ | (ว่าง) |

## หน้าจอ Log และ Wx

| คีย์ | หน้าที่โดยสรุป | ชนิดค่า | ค่าใน Template |
|---|---|---|---|
| `verbose` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 1 |
| `showDomain` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 0 |
| `showDomain_NPC` | ควบคุมการแสดงผล หน้าต่าง และ Log | ข้อความหรือรายการ | parseMsg_presence |
| `showDomain_Shop` | ควบคุมการแสดงผล หน้าต่าง และ Log | ข้อความหรือรายการ | list |
| `squelchDomains` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `verboseDomains` | ควบคุมการแสดงผล หน้าต่าง และ Log | ค่าเปล่า/ข้อความ | (ว่าง) |
| `beepDomains` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `beepDomains_notInTown` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `friendlyAID` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `showTime` | ควบคุมการแสดงผล หน้าต่าง และ Log | ค่าเปล่า/ข้อความ | (ว่าง) |
| `showTimeDomains` | ควบคุมการแสดงผล หน้าต่าง และ Log | ค่าเปล่า/ข้อความ | (ว่าง) |
| `showTimeDomainsFormat` | ควบคุมการแสดงผล หน้าต่าง และ Log | ค่าเปล่า/ข้อความ | (ว่าง) |
| `wx_map_maxAutoSize` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 300 |
| `wx_map_monsterSticking` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 1 |
| `wx_map_npcSticking` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 1 |
| `wx_map_playersSticking` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 1 |
| `wx_map_portalSticking` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 5 |
| `wx_map_route` | ควบคุมการแสดงผล หน้าต่าง และ Log | ค่าเปล่า/ข้อความ | (ว่าง) |
| `wx_map_namesDetail` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 8 |
| `wx_map_playerNameZoom` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 8 |
| `wx_map_partyNameZoom` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 1 |
| `wx_map_portalDestinations` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 0 |
| `wx_npcTalk` | ควบคุมการแสดงผล หน้าต่าง และ Log | ค่าเปล่า/ข้อความ | (ว่าง) |
| `wx_captcha` | ควบคุมการแสดงผล หน้าต่าง และ Log | ค่าเปล่า/ข้อความ | (ว่าง) |
| `showAllDamage` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 0 |
| `logChat` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 1 |
| `logPrivateChat` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 1 |
| `logPartyChat` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 1 |
| `logGuildChat` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 1 |
| `logClanChat` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 0 |
| `logSystemChat` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 1 |
| `logLocalBroadcast` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 1 |
| `logShop` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 1 |
| `logEmoticons` | ควบคุมการแสดงผล หน้าต่าง และ Log | ค่าเปล่า/ข้อความ | (ว่าง) |
| `logConsole` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 1 |
| `logAppendUsername` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 1 |
| `logAppendServer` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 0 |
| `monsterLog` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `playerLog` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `logDead` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 1 |
| `questDisplayStyle` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 2 |
| `chatTitleOversize` | ควบคุมการแสดงผล หน้าต่าง และ Log | ตัวเลข | 0 |
| `shopTitleOversize` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `buyerShopTitleOversize` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `sleepTime` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 10000 |
| `ignoreAll` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `itemHistory` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 0 |
| `portalCompile` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `portalRecord` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 2 |
| `portalRecord_recompileAfter` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `portalUpdatePosition` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ตัวเลข | 1 |
| `npcTimeResponse` | คีย์ย่อยของหมวดที่เกี่ยวข้อง | ค่าเปล่า/ข้อความ | (ว่าง) |
| `logToFile_Debug` | ควบคุมการแสดงผล หน้าต่าง และ Log | ค่าเปล่า/ข้อความ | (ว่าง) |
| `logToFile_Errors` | ควบคุมการแสดงผล หน้าต่าง และ Log | ค่าเปล่า/ข้อความ | (ว่าง) |
| `logToFile_Messages` | ควบคุมการแสดงผล หน้าต่าง และ Log | ค่าเปล่า/ข้อความ | (ว่าง) |
| `logToFile_Warnings` | ควบคุมการแสดงผล หน้าต่าง และ Log | ค่าเปล่า/ข้อความ | (ว่าง) |

## แหล่งอ้างอิง

- [config.txt ฉบับต้นฉบับ](https://github.com/OpenKore/openkore/blob/master/control/config.txt)
- [หมวด Config บน OpenKore Wiki](https://openkore.com/wiki/Category:Config.txt)
