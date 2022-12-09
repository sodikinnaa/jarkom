# jarkom
![image](https://user-images.githubusercontent.com/80803209/206598021-1ab1df07-d37e-4a38-905f-b01760d1ad65.png)

#Router 0
>Router>enable
Router#configure
Router(config)#interface fa0/0
Router(config-if)#ip add 192.168.1.1 255.255.255.0
Router(config-if)#no shutdown
%LINK-5-CHANGED: Interface FastEthernet0/0, Change state to up
Router(config-if)#exit
Router(config)

Router(config)#interface fa0/1
Router(config-if)#ip add 192.168.100.1 255.255.255.0
Router(config-if)#no shutdown
%LINK-5-CHANGED: Interface FastEthernet0/1, Change state to up
Router(config-if)#exit
Router(config)

#Router 1 
Router>enable
Router#configure
Router(config)#int fa0/0
Router(config-if)#ip add 192.168.1.2 255.255.255.0
Router(config-if)#no shutdown
%LINK-5-CHANGED: Interface FastEthernet0/0, Change state to up
%LINEPROTO-5-UPDOWN: Line protocol on Interface FastEthernet0/0 change state to up
Router(config-if)#exit
Router(config)#int fa0/1
Router(config-if)#ip add 192.168.200.1 255.255.255.0
Router(config-if)#no shutdown
%LINK-5-CHANGED: Interface FastEthernet0/1, Change state to up

Router(config-if)#exit
Router(config)


#Routing
#ip route <destination><subnet mask><next hop address>
  
