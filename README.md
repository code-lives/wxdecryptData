# 微信小程序手机号解密

# 初始化
$WXgetPhone = new \WXBizDataCrypt\Phone\WXgetPhone($appid,$session_key);

## 这是解密 data是空
$errCode=$WXgetPhone->decryptData($encryptedData, $iv, $data);

## 结果

$errCode ==0   表示解密成功

$data = json_decode($data, true);
