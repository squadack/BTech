set (BTCommon_SRCS
	Action.cpp
	AttackObject.cpp
	Base/MechBase.cpp
	Base/MechPartBase.cpp
	Base/WeaponBase.cpp
	BiHash.cpp
	BTMapManager.cpp
	Colors.cpp
	DataManager.cpp
	Effect.cpp
	EnumHashFunctions.h
	GraphicsEntity.cpp
	GraphicsFactory.cpp
	GraphicsHex.cpp
	GraphicsMap.cpp
	Grid.cpp
	Hex.cpp
	InfoBar.cpp
	Map.cpp
	Mech.cpp
	MechEntity.cpp
	MechPart.cpp
	MechWarrior.cpp
	Model/MechModel.cpp
	Model/WeaponModel.cpp
	MoveObject.cpp
	Objects.cpp
	Paths.cpp
	Player.cpp
	Position.cpp
	Rules.cpp
	Settings.cpp
	TerrainTileModel.cpp
	Tile.cpp
	TileManager.cpp
	Utils.cpp
	Weapon.cpp
)

set (BTCommon_HDRS
	BTMapManager.h
	GraphicsEntity.h
	GraphicsHex.h
	GraphicsMap.h
	InfoBar.h
	MechEntity.h
	Model/MechModel.h
	Model/WeaponModel.h
	Objects.h
	Player.h
	Rules.h
)

qt5_wrap_cpp (BTCommon_SRCS ${BTCommon_HDRS})

add_library (BTCommon ${BTCommon_SRCS})
target_link_libraries (BTCommon ${Qt5Widgets_LIBRARIES})
