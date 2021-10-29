# TheLibraries
--------------
TheLibrary-WPF
--------------
TheSystem.dll
TheSystem
{
  Time (Start, End)
  Systems : Actors
  Actions
}
System : Actor
{
  Thread (Main, Other)
  Dimensions
  {
    Time : Dimension
    Actors : Dimension
    Acts : Dimension
  }
}
TheSystem : Singleton<System>
Product : System
{
  Initialize
  Start
  Stop
}
Event : Link<Actor, Act, Time>
Act : IAct
Link
{
  Object1
  Object2
}
Dimension
{
  Items
}
