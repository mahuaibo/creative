### TODO LIST

```
1) DeleteBuyer & ModifyBuyer Unrealized.
```

### Model 

User
```
type User struct {
 	Username    string `json:"username"`
 	Email       string `json:"email"`
    Address     string `json:"address"` 
}
```

Artist
```
type Artist struct {
 	Name        string `json:"name"`
 	Desc        string `json:"desc"`
    Username    string `json:"username"` 
}
```

Production
```
type Production struct { 
    Type                  string            `json:"type"` 
    Serial                string            `json:"serial"` 
    Name                  string            `json:"name"` 
    Desc                  string            `json:"desc"` 
    CopyrightPriceType    string            `json:"copyright_price_type"` 
    CopyrightPrice        string            `json:"copyright_price"`      
    CopyrightNum          string            `json:"copyright_num"`         
    Username              string            `json:"username"` 
    Supporters            map[string]string `json:"supporters"`
    Buyers                map[string]string `json:"buyers"` 
    CopyrightTransferPart string            `json:"copyright_transfer_part"`  
}
```

# Invoke func

```
1）AddUser
2）DeleteUser
3）ModifyUser
4）QueryUser
5）ListOfUser
6）AddArtist
7）DeleteArtist
8）ModifyArtist
9）QueryArtist
10）ListOfArtist
11）AddProduction
12）DeleteProduction
13）ModifyProduction
14）QueryProduction
15）ListOfProduction
16）ListOfSupporter
17）AddSupporter
18）AddBuyer
19）ListOfBuyer
20）DeleteBuyer
21）ModifyBuyer
```

### Token & Address

```
{
    Token: "70698e364537a106b5aa5332d660e2234b37eebcb3768a2a97ffb8042dfe2fc4"
    Address: "07caf88941eafcaaa3370657fccc261acb75dfba"
}, {
    Token: "344c267e5acb2ac9107465fc85eba24cbb17509e918c3cc3f5098dddf42167e5"
    Address: "a5ff00eb44bf19d5dfbde501c90e286badb58df4"
}, {
    Token: "bc4bcb06a0793961aec4ee377796e050561b6a84852deccea5ad4583bb31eebe"
    Address: "4230a12f5b0693dd88bb35c79d7e56a68614b199"
}
```g

### Scripts

```
func_init.sh 
func_user.sh
func_artist.sh
func_production.sh
func_token.sh
initialization.sh
test.sh
```
