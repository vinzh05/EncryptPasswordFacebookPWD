# EncryptPasswordFacebookPWD

This is an encrypted facebook password built from .Net Core to .Net Framework

If you find it good, please give me 1 star and 1 fork

// The values of publicKey,keyId,version are from shared_data.

// You need to call https://www.instagram.com/data/shared_data/ to get shared_data first.

Example Request:

JObject jObject = JObject.Parse(response);

string key_id = jObject.SelectToken("encryption.key_id")?.ToString();

string public_key = jObject.SelectToken("encryption.public_key")?.ToString();
