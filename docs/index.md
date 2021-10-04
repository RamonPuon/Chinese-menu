<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <style>
        
        @import "{{site.theme}}";
        header{
        display: none;
        }
        @import url('https://fonts.googleapis.com/css2?family=Single+Day&display=swap');
        
        .body{
            margin:0;
            font-family: 'Single Day', cursive;
        }

        .grid{
            display: grid;
            grid-template-columns: repeat(5, 1fr);
            grid-template-rows: repeat(4, minmax(100px, auto));
            background: pink;
        }
        
        .item{
            display: grid;
            grid-column: 2/5;
            grid-row: 3/4;
            background: pink;
            grid-template-columns: subgrid;
            grid-template-rows: repeat(3, minmax(80px,auto));
            gap: 12px;
        }

        .sub-item{
            display: grid;
            grid-template-columns: 1fr;
            grid-template-rows: repeat(3,minmax(80px,auto));
            background: papayawhip;
            justify-items: center;
            align-items: center; 
            border-radius: 8px;           
        }

        .sub-item:nth-child(2n+1) {
            background: lightyellow;
        }

        .sub-item img{
            object-fit: cover;
            width: 100px;
        }
        .sub-item > p{
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .sub-item > p span:first-child{
            font-size: 20px;
        }

        @media (max-width: 640px){
            .grid{
                grid-template-columns: 80px 1fr 80px;
            }
            .item{
                grid-column: 2/3;
                grid-row: 3/4;
                grid-template-columns: subgrid;
            }
        


    </style>
</head>
<body>
    <div class="grid">
        <h3 class="title">Chinese menu</h3>

        <div class="item">
            <div class="sub-item">
                <p>
                    <span>Jiaozi</span>
                    <span>饺子</span>
                </p>
                <img src="https://cdn-icons-png.flaticon.com/512/1690/1690702.png" alt="jiazi">
                <p>$15,00</p>
            </div>
    
            <div class="sub-item">
                <p>
                    <span>Chunjuan</span>
                    <span>春卷</span>
                </p>
                <img src="https://cdn-icons-png.flaticon.com/512/3447/3447898.png" alt="roll">
                <p>$8,00</p>
            </div>
    
            <div class="sub-item">
                <p>
                    <span>Miantiao</span>
                    <span>面条</span>
                </p>
                <img src="https://cdn-icons-png.flaticon.com/512/1623/1623675.png" alt="noodle">
                <p>$22,00</p>
            </div>
    
            <div class="sub-item">
                <p>
                    <span>Baozi</span>
                    <span>包子</span>
                </p>
                <img src="https://cdn-icons-png.flaticon.com/512/1357/1357304.png" alt="baozi">
                <p>$12,00</p>
            </div>
    
            <div class="sub-item">
                <p>
                    <span>Mifan</span>
                    <span>米饭</span>
                </p>
                <img src="https://cdn-icons-png.flaticon.com/512/541/541705.png" alt="rice">
                <p>$8,00</p>
            </div>
    
            <div class="sub-item">
                <p>
                    <span>Yuebing</span>
                    <span>月饼</span>
                </p>
                <img src="https://cdn-icons-png.flaticon.com/512/3447/3447998.png" alt="cake">
                <p>$6,00</p>
            </div>
    
            <div class="sub-item">
                <p>
                    <span>Cha</span>
                    <span>茶</span>
                </p>
                <img src="https://cdn-icons-png.flaticon.com/512/3504/3504747.png" alt="tea">
                <p>$7,00</p>
            </div>
    
            <div class="sub-item">
                <p>
                    <span>Huangjiu</span>
                    <span>黄酒</span>
                </p>
                <img src="https://cdn-icons-png.flaticon.com/512/3766/3766698.png" alt="drink">
                <p>$15,00</p>
            </div>
    
            <div class="sub-item">
                <p>
                    <span>Sachima</span>
                    <span>沙琪玛</span>
                </p>
                <img src="https://cdn-icons-png.flaticon.com/512/890/890082.png" alt="sachima">
                <p>$12,00</p>
            </div>
    
        </div>

    </div>
</body>
</html>
