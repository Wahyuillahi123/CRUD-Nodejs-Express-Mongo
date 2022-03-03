# CRUD Nodejs Express Mongo
CRUD Nodejs Express dan MongoDB

## Get
``` html
  Database.fine(function(){
    //semua data
  });

  Database.fineById(req.params.idData,function(err,data){
    //satu data berdasarkan id
  });

  Database.fineOne({token:token,sesi:sesi}).then(data=>{
    //satu data berdasarkan suatu nilai selain id;
  });

```

## Post
``` html
  const newData=Data({
    nama:nmdepan+' '+nmbelakang,
    usia:umur
  });
  newData.save().then(data=>{
    //menyimpan data ke database;
  });
```

## Update
``` html
  Database.findByIdUpdate(req.params.idData,{usia:'20',jenkel:'Leki laki'},function(err){
    if(err){
      console.log(err)
    }else{
      //mengupdate data berdasarkan id;
    }
  });

  Database.findByOneUpdate({alamat:'barau barau 1',rt:'20'},{usia:'20',jenkel:'Leki laki'},function(err){
    if(err){
      console.log(err)
    }else{
      //mengupdate data berdasarkan suatu nilai selain id;
    }
  });
```

## Delete
``` html
  Database.findByIdDelete(req.params.idData,function(){
    //menghapus data dari daabase;
  });
```

# Support
Follow my instagram : https://www.instagram.com/wahyu_illahi07/ 
Youtube Channel : https://www.youtube.com/playlist?list=PL2DC6n3PrEKVXN9nvzONe9idXa9BgCusj

