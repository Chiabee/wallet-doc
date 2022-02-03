# wallet-doc

源代码将在之后提供。 此应用程序处于内测阶段，请勿用于正式用途。

The source code would available later. This app is in ALPHA stage, don't use in PRODUCTION.

Please scroll down for the English description.

# 说明

## 当前版本
Chiabee Wallet [0.1.3519.220202] 


## 特色功能

- 初始创建为12位的助记词，并可将这12位助记词转成24位助记词导入Chia官方全节点钱包和轻钱包。
- 可导入Chia的24位助记词。
- 同一助记词下的多钱包管理（类似metamask）

## 基本功能

- 支持离线钱包
- 可接收XCH和CATs的资产。（目前已添加的CATs有BSH\SBX\CH21）
- 可创建影子钱包。即：同样的助记词，加密码和不加密码将是两个不同的私钥（钱包）。本功能适合专业人士使用。

## 待实现功能

- 暂不支持发送资产
- 暂时无法读取可变地址上的资产
- 缺少提示功能（如删除提示、密码错误提示等）

## 首次创建流程
1. 创建你的钱包密码。

    ![image](https://user-images.githubusercontent.com/80501701/152331288-f9d9d2db-39bc-4685-82bd-8dc012bcd436.png)

1. 可以选择导入助记词，或创建新的助记词。

    ![image](https://user-images.githubusercontent.com/80501701/152331434-d080093b-c8b0-4cba-bae9-189562bda965.png)
    
   - Import：可导入本钱包创建的12位助记词，或Chia客户端的24位助记词
  
    ![image](https://user-images.githubusercontent.com/80501701/152331486-38c6dde9-9a48-463d-bbf1-3fea4e6c5ff2.png)

   - Create：可创建一个12位助记词（该助记词可生成被Chia客户端识别的24位助记词，后面会再提到）

    ![image](https://user-images.githubusercontent.com/80501701/152331556-730d383b-c7a2-49a4-8a0b-18f740caf214.png)

1. 点击confirm后即进入钱包主页

    ![image](https://user-images.githubusercontent.com/80501701/152331589-9e41fba0-9842-45c7-84cb-01db2b815dea.png)

1. 右上角会显示钱包名称和指纹。点击此处可查看钱包信息

    ![image](https://user-images.githubusercontent.com/80501701/152331633-6d025c6e-c349-4eb4-acf8-371d38741299.png)

   - 特别注意，由于目前还没有做删除提示，点击删除将直接删除本钱包。【如果你没有备份好助记词，请一定不要点击它！！！】

    ![image](https://user-images.githubusercontent.com/80501701/152331683-9960f9ea-74b9-482a-b29e-1f9830dc7d46.png)

   - 修改钱包名字
   
     ![image](https://user-images.githubusercontent.com/80501701/152331801-f56f678e-388f-4beb-ae3c-98badef36754.png)

   - 导出钱包基本信息，包括可被用于Chia客户端的24位助记词信息。
   
    ![image](https://user-images.githubusercontent.com/80501701/152331843-a115d2b6-852d-46d3-8443-03eea8c22642.png)
    ![image](https://user-images.githubusercontent.com/80501701/152331879-837cfd28-a0fc-41d9-a093-97d3223bda9d.png)

1. Add By Password：可创建带密码的影子钱包。【建议专业人士使用，后文会详细说明】
1. Add By Serial：可创建普通序列钱包。序列钱包是按顺序创建的，如果序列钱包被删除，重新创建时将恢复原本的序列钱包。

## 创建影子钱包（本功能适合专业人员使用）
- 影子钱包是一个带密码的助记词钱包。
- 同样的助记词，不带密码和带密码，对应的是不同的私钥（钱包）。
- 因此，对于一些专业人士而言，使用同一套助记词的情况下，可以选择用普通钱包存放少量钱，而用影子钱包存放更重要的资产。这样，哪怕助记词不小心被泄露，影子钱包也很难被人发现，从而保护使用者的资产。（此时也意味着应该将资产转移到一个新的安全钱包当中了！）
- Chiabee wallet的影子钱包是按密码及序列创建的。如果不小心将该钱包删除，只要在重新创建时输入之前的密码，就可将被删掉的影子钱包恢复出来。
- **特别强调：若使用影子钱包功能，除助记词外，还需要记住对应的影子钱包密码，否则影子钱包内的资产将彻底无法找回！**
    ![image](https://user-images.githubusercontent.com/80501701/152331921-afbef264-83c6-486b-8a2e-f0b52b63d0b4.png)
    ![image](https://user-images.githubusercontent.com/80501701/152331932-f904eecd-bfc7-40b9-a877-0b0a0dbd7228.png)
    ![image](https://user-images.githubusercontent.com/80501701/152331943-ae688aaa-86d7-4e5a-9251-e6244d470ef1.png)


## 特别注意
- 初次使用会提示要创建密码。如之后忘记密码，则只能通过助记词来恢复钱包。
- 若使用影子钱包功能，除助记词外，还需要记住对应的影子钱包密码，否则影子钱包内的资产将彻底无法找回。

# instruction

## current version
Chiabee Wallet [0.1.3519.220202]


## special function

- The initial creation is a 12-digit mnemonic, and the 12-digit mnemonic can be converted into a 24-digit mnemonic and imported into the Chia official full node wallet and light wallet.
- Chia's 24-digit mnemonic can be imported.
- Multi-wallet management under the same mnemonic (similar to metamask)

## basic skills

- Support offline wallet
- Assets that can receive XCH and CATs. (The currently added CATs are BSH\SBX\CH21)
- Ability to create shadow wallets. That is: the same mnemonic, encrypted and unencrypted will be two different private keys (wallets). This function is suitable for professionals.

## Functions to be implemented

- Currently does not support sending assets
- temporarily unable to read assets on variable addresses
- Lack of prompt function (such as deletion prompt, password error prompt, etc.)

## First create process
1. Create your wallet password.

    ![image](https://user-images.githubusercontent.com/80501701/152331288-f9d9d2db-39bc-4685-82bd-8dc012bcd436.png)

1. You can choose to import a mnemonic, or create a new mnemonic.

    ![image](https://user-images.githubusercontent.com/80501701/152331434-d080093b-c8b0-4cba-bae9-189562bda965.png)
    
   - Import: can import the 12-digit mnemonic created by this wallet, or the 24-digit mnemonic of the Chia client
  
    ![image](https://user-images.githubusercontent.com/80501701/152331486-38c6dde9-9a48-463d-bbf1-3fea4e6c5ff2.png)

   - Create: A 12-bit mnemonic can be created (this mnemonic can generate a 24-bit mnemonic recognized by the Chia client, which will be mentioned later)

    ![image](https://user-images.githubusercontent.com/80501701/152331556-730d383b-c7a2-49a4-8a0b-18f740caf214.png)

1. Click confirm to enter the wallet homepage

    ![image](https://user-images.githubusercontent.com/80501701/152331589-9e41fba0-9842-45c7-84cb-01db2b815dea.png)

1. The wallet name and fingerprint will be displayed in the upper right corner. Click here to view wallet information

    ![image](https://user-images.githubusercontent.com/80501701/152331633-6d025c6e-c349-4eb4-acf8-371d38741299.png)

   - Special attention, since there is no deletion prompt yet, clicking delete will delete the wallet directly. [If you don't have a backup of the mnemonic phrase, please don't click it! ! ! 】

    ![image](https://user-images.githubusercontent.com/80501701/152331683-9960f9ea-74b9-482a-b29e-1f9830dc7d46.png)

   - Modify wallet name
   
     ![image](https://user-images.githubusercontent.com/80501701/152331801-f56f678e-388f-4beb-ae3c-98badef36754.png)

   - Export basic wallet information, including 24-bit mnemonic information that can be used by Chia client.
   
    ![image](https://user-images.githubusercontent.com/80501701/152331843-a115d2b6-852d-46d3-8443-03eea8c22642.png)
    ![image](https://user-images.githubusercontent.com/80501701/152331879-837cfd28-a0fc-41d9-a093-97d3223bda9d.png)

1. Add By Password: Create a shadow wallet with a password. [It is recommended for professionals to use, and will be explained in detail later]
1. Add By Serial: You can create a common serial wallet. Sequence wallets are created in order. If the sequence wallet is deleted, the original sequence wallet will be restored when it is re-created.

## Create shadow wallet (this function is suitable for professionals)
- Shadow wallet is a mnemonic wallet with a password.
- The same mnemonic, without password and with password, corresponds to different private keys (wallets).
- Therefore, for some professionals, using the same set of mnemonic phrases, it is possible to choose to store a small amount of money in a normal wallet, and use a shadow wallet to store more important assets. In this way, even if the mnemonic is accidentally leaked, the shadow wallet is difficult to be discovered, thus protecting the user's assets. (This also means that the assets should be transferred to a new secure wallet!)
- The shadow wallet of Chiabee wallet is created by password and sequence. If you accidentally delete the wallet, you can restore the deleted shadow wallet as long as you enter the previous password when re-creating it.
- ** Special emphasis: If you use the shadow wallet function, in addition to the mnemonic phrase, you also need to remember the corresponding shadow wallet password, otherwise the assets in the shadow wallet will be completely impossible to retrieve! **
    ![image](https://user-images.githubusercontent.com/80501701/152331921-afbef264-83c6-486b-8a2e-f0b52b63d0b4.png)
    ![image](https://user-images.githubusercontent.com/80501701/152331932-f904eecd-bfc7-40b9-a877-0b0a0dbd7228.png)
    ![image](https://user-images.githubusercontent.com/80501701/152331943-ae688aaa-86d7-4e5a-9251-e6244d470ef1.png)


## pay attention
- You will be prompted to create a password when using it for the first time. If you forget the password later, you can only restore the wallet through the mnemonic phrase.
- If you use the shadow wallet function, in addition to the mnemonic phrase, you also need to remember the corresponding shadow wallet password, otherwise the assets in the shadow wallet will be completely irretrievable.
