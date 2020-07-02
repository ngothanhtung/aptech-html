<!DOCTYPE html>
<html>

<head>
    <title>SHOPPING CART EXAMPLE</title>
    <meta charset='utf-8'>
    <script src="https://code.jquery.com/jquery-2.1.3.js"></script>
    <link href="http://maxcdn.bootstrapcdn.com/bootstrap/3.3.1/css/bootstrap.min.css" rel="stylesheet">
    <script src="http://maxcdn.bootstrapcdn.com/bootstrap/3.3.1/js/bootstrap.min.js"></script>
    <style>
        body {
            margin: 20px;
        }

        .wrapper {
            width: 1140px;
            margin: 0 auto;
        }
    </style>
</head>

<body>
    <div class="wrapper">
        <h1>SHOPPING CART EXAMPLE</h1>
        <div class="row">
            <div class="col-md-4">
                <div class="img-thumbnail" style="border: 1px solid gray; width: 100%; height: 160px"></div>
                <div>
                    iPhone 6 Plus
                </div>
                <div>
                    Giá: 17.000.000đ
                </div>
                <button id="product-1" data-name="iPhone 6 Plus" data-price="17000000" class="add-to-cart btn btn-primary">Add to cart</button>
            </div>
            <div class="col-md-4">
                <div class="img-thumbnail" style="border: 1px solid gray; width: 100%; height: 160px"></div>
                <div>
                    Nokia Lumia 1520
                </div>
                <div>
                    Giá: 12.500.000đ
                </div>
                <button id="product-2" data-name="Nokia Lumia 1520" data-price="12500000" class="add-to-cart btn btn-danger">Add to cart</button>
            </div>
            <div class="col-md-4">
                <div class="img-thumbnail" style="border: 1px solid gray; width: 100%; height: 160px"></div>
                <div>
                    Samsung Galaxy Note 4
                </div>
                <div>
                    Giá: 18.500.000đ
                </div>
                <button id="product-3" data-name="Samsung Galaxy Note 4" data-price="18500000" class="add-to-cart btn btn-info">Add to cart</button>
            </div>
        </div>
        <br />
        <div class="row">
            <table class="table table-bordered" id="table-products">
                <thead>
                    <tr>
                        <th>Id</th>
                        <th>Name</th>
                        <th>Price</th>
                        <th>Quantity</th>
                        <th>Total</th>
                    </tr>
                </thead>
                <tbody></tbody>
            </table>
        </div>
        <div>
            <button class="btn btn-lg btn-success" id="button-clear">Clear</button>
        </div>
        <div class="text-right">

            <hr />
            <address>
                Developed by Ngo Thanh Tung - Softech Aptech
            </address>
        </div>
    </div>
</body>
</html>

<script>
    // Định nghĩa một mảng các phần tử sẽ bỏ vào giỏ hàng
    var shoppingCartItems = [];

    $(document).ready(function () {
        // Kiểm tra nếu đã có sessionStorage["shopping-cart-items"] hay chưa?
        if (sessionStorage["shopping-cart-items"] != null) {
            shoppingCartItems = JSON.parse(sessionStorage["shopping-cart-items"].toString());
        }

        // Hiển thị thông tin từ giỏ hàng
        displayShoppingCartItems();
    });


    // Sự kiện click các button có class=".add-to-cart"
    $(".add-to-cart").click(function () {
        var button = $(this); // Lấy đối tượng button mà người dùng click
        var id = button.attr("id"); // id của sản phẩm là id của button
        var name = button.attr("data-name"); // name của sản phẩm là thuộc tính data-name của button
        var price = button.attr("data-price"); // price của sản phẩm là thuộc tính data-price của button
        var quantity = 1; // Số lượng


        var item = {
            id: id,
            name: name,
            price: price,
            quantity: quantity
        };

        var exists = false;
        if (shoppingCartItems.length > 0) {
            $.each(shoppingCartItems, function (index, value) {
                // Nếu mặt hàng đã tồn tại trong giỏ hàng thì chỉ cần tăng số lượng mặt hàng đó trong giỏ hàng.
                if (value.id == item.id) {
                    value.quantity++;
                    exists = true;
                    return false;
                }
            });
        }

        // Nếu mặt hàng chưa tồn tại trong giỏ hàng thì bổ sung vào mảng
        if (!exists) {
            shoppingCartItems.push(item);
        }

        // Lưu thông tin vào sessionStorage
        sessionStorage["shopping-cart-items"] = JSON.stringify(shoppingCartItems); // Chuyển thông tin mảng shoppingCartItems sang JSON trước khi lưu vào sessionStorage
        // Gọi hàm hiển thị giỏ hàng
        displayShoppingCartItems();
    });

    // Xóa hết giỏ hàng shoppingCartItems
    $("#button-clear").click(function () {
        shoppingCartItems = [];
        sessionStorage["shopping-cart-items"] = JSON.stringify(shoppingCartItems);
        $("#table-products > tbody").html("");
    });


    // Hiển thị giỏ hàng ra table
    function displayShoppingCartItems() {
        if (sessionStorage["shopping-cart-items"] != null) {
            shoppingCartItems = JSON.parse(sessionStorage["shopping-cart-items"].toString()); // Chuyển thông tin từ JSON trong sessionStorage sang mảng shoppingCartItems.

            $("#table-products > tbody").html("");
            // Duyệt qua mảng shoppingCartItems để append từng item dòng vào table
            $.each(shoppingCartItems, function (index, item) {
                var htmlString = "";
                htmlString += "<tr>";
                htmlString += "<td>" + item.id + "</td>";
                htmlString += "<td>" + item.name + "</td>";
                htmlString += "<td style='text-align: right'>" + item.price + "</td>";
                htmlString += "<td style='text-align: right'>" + item.quantity + "</td>";
                htmlString += "<td style='text-align: right'>" + item.price * item.quantity + "</td>";
                htmlString += "</tr>";

                $("#table-products > tbody:last").append(htmlString);

            });
        }
    }
</script>