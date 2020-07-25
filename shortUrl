javascript:(function() {
        const long_url = prompt('1')
        const xhr = new XMLHttpRequest();
        xhr.onreadystatechange = function(){
            if( xhr.readyState === 4){
                if( xhr.status >= 200 && xhr.status < 300 || xhr.status === 304){
                    const data = xhr.responseText;
                    const url = JSON.parse(data).ae_url
                    alert(url)
                }
            }
        };
        xhr.open("get", 'https://api.uomg.com/api/long2dwz?dwzapi=suoim&url=' + long_url, true);
        xhr.send(null);
})();
