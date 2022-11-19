
# Hypervisor<br>

하이퍼바이저는 물리적 하드웨어에 설치된 소프트웨어 계층으로, 물리적 머신을 다수의 가상 머신으로<br>
분할 할 수 있도록 해줍니다. 하이퍼바이저를 이용하면 동일한 물리적 하드웨어에서 여러 운영 체제를<br>
동시에 실행할 수 있습니다. 가상 머신에 설치된 운영 체제는 게스트 OS라고 부르며 경우에 따라<br>
인스턴스라고 부를 때도 있습니다. 또한 하이퍼바이저가 실행되는 하드웨어는 호스트 머신이라고 부릅니다.<br>
가상 머신 매니저(VMM)라고도 부르는 하이퍼바이저 관리 콘솔은 가상 머신을 쉽게 관리할 수 있도록<br>
도와주는 컴퓨터 소프트웨어입니다.<br><br>

<img src="https://img.alicdn.com/tfs/TB1IZBKDVYqK1RjSZLeXXbXppXa-1152-1213.png_.webp" width="400" height="421"/><br><br>

## 하이퍼바이저 유형<br>

하이퍼바이저에는 제1형과 제2형으로 구분되는 두 가지 유형이 있습니다.<br>
제1형 하이퍼바이저는 네이티브 또는 베어메탈 하이퍼바이저라고도 부르며, 하드웨어에 직접 설치되어<br>
하드웨어를 게스트 OS를 설치할 수 있는 여러 개의 가상 머신으로 분할해줍니다.<br>
가상 머신 관리 소프트웨어를 통해 이 하이퍼바이저를 관리할 수 있으며, 여러 게스트 OS가<br>
현재 리소스 요건에 따라 물리적 서버 사이에서 자동으로 이동할 수 있습니다.<br>

### 제1형 하이퍼바이저<br>

- 내결함성: 물리적 서버에 장애가 발생하면 관리 소프트웨어는 이용 가능한 다른 서버로 신속하게<br>
인스턴스를 마이그레이션하여 물리적 하드웨어에 장애가 발생했다는 것조차 알 수 없도록 조치합니다.<br>
사용자는 어떤 서비스 중단도 느낄 수 없으며 장애가 발생한 하드웨어는 유지보수 및 운영 직원이<br>
편한 시간에 수리 또는 교체할 수 있습니다.<br>

- RAM 용량 초과/동적 할당: 서버에서 여러 인스턴스를 실행할 때 가상 머신에 할당되는 전체 RAM을<br>
기반 하드웨어의 전체 물리적 메모리 용량보다 큰 값으로 설정할 수도 있습니다.<br><br>

- 1형의 하이퍼바이저에는 Xen, Oracle VM Server for SPARC, Oracle VM Server for x86, Microsoft Hyper-V 및<br>
VMware의 ESX / ESXi가 있습니다.<br><br>

<img src="https://img.alicdn.com/tfs/TB1jm0MDYvpK1RjSZFqXXcXUVXa-1625-1221.png_.webp" width="500" height="421"/><br><br>

### 제2형 하이퍼바이저<br>

호스트 하이퍼바이저라고도 부르며 호스트의 운영 체제 내에 설치되기 때문에 하이퍼바이저 관리 콘솔이<br>
필요하지 않다는 장점이 있습니다. 제2형 하이퍼바이저는 RAM의 초과/동적 할당을 지원하지 않으므로,<br>
가상 머신에 리소스를 할당할 때 주의해야 합니다.<br><br>

- 2형의 하이퍼바이저에는 VMware Workstation, VMware Player, VirtualBox 및 Parallels Desktop for Macdl 있습니다.<br><br>

<img src="https://img.alicdn.com/tfs/TB1d2lVDZfpK1RjSZFOXXa6nFXa-1632-1207.png_.webp" width="500" height="421"/><br><br>