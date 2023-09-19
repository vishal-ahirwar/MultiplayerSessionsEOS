# MultiplayerSessionsEOS

## Make sure to enable plugin first then edit defaultEngine.ini add the below script to defaultEngine.ini and package the project in shiping mode

```
  [OnlineSubsystemEOS]
    bEnabled=true

    [OnlineSubsystem]
    DefaultPlatformService=EOS

    [/Script/Engine.GameEngine]
+NetDriverDefinitions=(DefName="GameNetDriver",DriverClassName="OnlineSubsystemEOS.NetDriverEOS",DriverClassNameFallback="OnlineSubsystemUtils.IpNetDriver")

    [/Script/OnlineSubsystemEOS.NetDriverEOS]
    bIsUsingP2PSockets=true

```
