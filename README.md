# Dragonslayers
mauRong = 100;
mauNguoi = 100;
stRong = 33;
stNguoi = 49;
random = Math.random()*100;
agiRong = 33;
agiNguoi = 66;

function gietNo(agi, random) {
 if(agi > random) {
 	giet = true;
 	alert('Chết nè');
 }else {
 	giet = false;
	 alert('Tao đang mắc ỉa, tha cho mày đó');
 }
 return giet;
}

function gaySatThuong(mauHienTai, satThuong) {
 mauHienTai = mauHienTai - satThuong;
 return mauHienTai;
}

tieptuc = true;
alert('Trò chơi bắt đầu');
while (tieptuc){
   giet = true;
   alert('Đây là lượt của Dũng Sĩ');
   random = Math.random()*100;
   gietNo(agiNguoi, random);
   if(giet === true){
    alert('Tao giết mày nè Rồng')
    mauRong = gaySatThuong(mauRong, stNguoi);
   if(mauRong === 0){
    alert('Hết máu nè con');
   }else{
   	alert('1 cú móc chuẩn mực, Rồng chỉ còn ' + mauRong + ' máu');
   }
   }else {
    alert('Tới mày đó, ngon vô đây');
   }
   if(mauRong <= 0){
    tieptuc = false;
    alert('Con rồng chó chết đã tiêu đời');
   }else{
   giet = true;
   alert('Đây là lượt của Rồng');
   random = Math.random()*100;
   gietNo(agiNguoi, random);
   if(giet === true){
    alert('Tao sẽ cắn gãy chân mày Dũng Sĩ kia')
    mauNguoi = gaySatThuong(mauNguoi, stRong);
   if(mauNguoi === 0){
    alert('Mày chỉ còn là cái xác khô thôi');
   }else{
   	alert('1 cú táp rất đẹp, Dũng Sĩ chỉ còn ' + mauNguoi + ' máu');
   }
   }else {
   alert('Tới mày đó, ngon vô đây');
   }
if(mauNguoi <= 0){
   tieptuc = false;
   alert('Thằng Dũng Sĩ Đã Gãy');
}
   }
};
# Dragonslayers
