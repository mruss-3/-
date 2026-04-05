@startuml
left to right direction

actor "Дед" as Grandpa
actor "Баба" as Grandma
actor "Мышь" as Mouse
actor "Курочка" as Chicken

package "Управление золотыми активами" {
  usecase "Бить золотое яйцо" as Hit
  usecase "Разбить (случайно)" as BreakByTail
  usecase "Плакать" as Cry
  usecase "Утешить (Обещать простое)" as Comfort
  usecase "Снести простое яйцо" as SpawnSimple
}

' Дед и Баба бьют яйцо (действие)
Grandpa --> Hit
Grandma --> Hit

' Мышь разбивает (действие)
Mouse --> BreakByTail

' Дед и Баба ПЛАЧУТ (линии ведут к ним)
Grandpa --> Cry
Grandma --> Cry

' Курочка УТЕШАЕТ и СНОСИТ (линии к ней)
Chicken --> Comfort
Chicken --> SpawnSimple

' Зависимости внутри системы
Cry <.. Comfort : <<extend>> : если плачут
Comfort ..> SpawnSimple : <<include>>
@enduml