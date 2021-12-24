# Herobrine-NPC
==================================================

Comandos elaborados por SyRAFAELyS
Omlet:sy_rafael_ys

necessario: Operador, modo criativo e teclado com função de copiar e colar embutido
Como usar: Você precisará sumonar um NPC com o comando "/summon npc", no criativo edite o NPC em "configurações avançadas/adicionar comando". Para cada botão é necessario colar apenas o respectivo trecho de comandos pertencente a ele. Todos trechos de comandos tem que estar em "modo de botão"

==================================================

Botão 1: INICIAR

/tellraw @a {"rawtext":[{"text":"§eHerobrine entrou no jogo"}]} 
/setblock 1~ chest 
/tag @p[r=5] add SafeHBrine 
/tell @p[r=5] §aVocê recebeu a tag "SafeHBrine". As trolagens não surgirão em você ;D 

Botão 2: DROP DE ITENS

/tp @e[name=DropInt] ~-800 
/execute @a[tag=!SafeHBrine] ~ summon bat ~2 dried_out DropInt 
/effect @e[name=DropInt] slowness 999 100 true 
/effect @e[name=DropInt] invisibility 9999 1 true 
/tickingarea add 100 1 100  100 1 100 DropItem241 
/clone 1~ 1~ 100 0 100 
/execute @e[name=DropInt] ~ summon lightning_bolt ~1 
/execute @e[name=DropInt] ~ clone 100 0 100 100 0 100 ~ 
/execute @e[name=DropInt] ~ fill -1-1 ~1~1~1 air 1 destroy 
/execute @e[name=DropInt] ~~ kill @e[type=item,name=Baú,r=5] 
/tp @e[name=DropInt] ~-800 

Botão 3: TOTEM

/execute @a[tag=!SafeHBrine] ~ summon bat ~~10 attacked MarcHbrine 
/execute @e[name=MarcHbrine] ~~ fill 1-1~2 -1-1~4 monster_egg 5 
/execute @e[name=MarcHbrine] ~ fill 12 ~-1~4~4 light_block 15  
/execute @e[name=MarcHbrine] ~~ setblock 1-1~2 stone  
/execute @e[name=MarcHbrine] ~ setblock 1-1~4 stone 
/execute @e[name=MarcHbrine] ~ setblock -1-1~2 stone  
/execute @e[name=MarcHbrine] ~ setblock -1-1~4 stone  
/execute @e[name=MarcHbrine] ~ setblock 12 wither_rose  
/execute @e[name=MarcHbrine] ~~ setblock -14 wither_rose 
/execute @e[name=MarcHbrine] ~~ fill ~~3 ~~3~3 netherrack 
/execute @e[name=MarcHbrine] ~~ fill 1~2~3 ~-1~2~3 netherrack 
/execute @e[name=MarcHbrine] ~~ setblock ~2~4 skull 3 
/execute @e[name=MarcHbrine] ~~ setblock ~2~2 skull 2 
/execute @e[name=MarcHbrine] ~~ summon lightning_bolt ~4~3 
/execute @e[name=MarcHbrine] ~~ summon lightning_bolt -1~4~3 
/tp @e[name=MarcHbrine] ~-800~

Botão 4: HORDA

/execute @a[tag=!SafeHBrine] ~ summon bat ~ attacked HordaSkull 
/effect @e[name=HordaSkull] slowness 9999 100 true 
/effect @e[name=HordaSkull] invisibility 9999 1 true 
/difficulty 2 
/execute @e[name=HordaSkull] ~ summon skeleton ~2~5 
/execute @e[name=HordaSkull] ~~ summon skeleton 7~2 
/execute @e[name=HordaSkull] ~ summon skeleton -9~ 
/execute @e[name=HordaSkull] ~ summon skeleton 4~2-3 
/execute @e[name=HordaSkull] ~ summon skeleton ~2-10 
/execute @e[name=HordaSkull] ~ effect @e[type=skeleton,r=15] invisibility 9999 1 true 
/execute @e[name=HordaSkull] ~ effect @e[type=skeleton,r=15] resistance 9999 2 true 
/execute @e[name=HordaSkull] ~ replaceitem entity @e[type=skeleton,r=15] slot.armor.head 1 skull 
/execute @e[name=HordaSkull] ~ replaceitem entity @e[type=skeleton,r=15] slot.weapon.mainhand 1 air 
/tp @e[name=HordaSkull] ~-800

Botão 5: SE AFETAR

/tag @p[r=6] remove SafeHBrine 
/tell @p[r=5] §cTome cuidado. Todas trolagens surtirão efeito em você

Botão 6: VESTÍGIOS OFF

/fill -1-1 ~1~3~1 air 1 replace beehive  
/fill ~-1-1 ~1~3~1 air 1 replace chest  
/kill @e[type=item,r=5] 
/tp @e[type=npc,r=1] ~-800~  
/kill @e[type=npc,r=1]

========================================================
INFO dos botões:
INICIAR: Te protege de traps, chama Herobrine e ativa o drop de item. 
DROP DE ITENS: Dropa itens colocados no baú para os jogadores.
TOTEM: Gera estruturas de cruz para os jogadores.
HORDA: Spawna 5 crânios flutuantes que atacam os jogadores.
SE AFETAR: As traps surgirão em você também. 
VESTÍGIOS OFF: Mata o NPC e destroi o drop de itens.
========================================================
