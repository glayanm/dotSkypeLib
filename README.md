# dotSkypeLib
dot net skype Api lib


�ϥΤ�k

    DotSkype dotSkype = new DotSkype();

    //�n�J��SKYPE�b���K�X
    var loginToken = dotSkype.SendSoapLogin("xxxxxx", "password");

    //�洫SKYPETOKEN
    var exchangeToken = dotSkype.ExchangeSkypeToken(loginToken);

    //�d�ߦۤv��UserId
    var userName = dotSkype.GetSkypeUserProfile(exchangeToken);

    //�d�ߦۤv���B�ͲM��
    var contact = dotSkype.GetSkypeUserContactInfoList(userName, exchangeToken);

    //�d�ߦۤv���Ҧ�Conversaction
    //dotSkype.QueryThread(exchangeToken, "");

    //�e�j�q�T�O�����H��
    //dotSkype.SendMultipleText(exchangeToken, "test", new List<string>() { "sendMessageUserId" });

    //�e��ʫH��
    //dotSkype.SendText(exchangeToken, "test","sendMessageUserId");
