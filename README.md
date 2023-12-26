 const fs=require('fs');
fs.unlinkSync('importexport/index.js');

fs.unlinkSync('importexport/oper.js');
fs.rmdirSync('importexport');
fs.mkdir('revati',()=>{
    console.log('folder is created');
});
fs.writeFile('revati/bio.txt','r',()=>{
    console.log('file is created');
});
fs.readFile('revati/bio.txt','utf-8',(data,err)=>{
    if(err){
        console.log(err);
    }
    console.log(data);
})
fs.mkdirSync('importexport');
fs.writeFileSync('importexport/index.js','hello');
fs.unlinkSync('importexport/index.js');
fs.mkdir('modwrapfun',(err)=>{
    console.log('folder is created');
});
fs.writeFile('modwrapfun/wrap.js','hello',(err)=>{
    console.log();
});
fs.mkdir('httpserver',()=>{
    console.log('folder is created');
});

fs.unlink('revati/bio.txt',(err)=>{
    console.log('file is deleted');
});
fs.mkdir('practice',(err)=>{
    console.log('folder is created');
});
fs.writeFile('practice/exe.js','hello',(err)=>{
    console.log('file is created');
});
