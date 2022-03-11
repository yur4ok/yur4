var isValidNewBlock = (newBlock, previousBlock) => {
    if (previousBlock.index + 1 !== newBlock.index) {
        console.log('неверный индекс');
        return false;
    } else if (previousBlock.hash !== newBlock.previousHash) {
        console.log('неверный хеш предыдущего блока');
        return false;
    } else if (calculateHashForBlock(newBlock) !== newBlock.hash) {
        console.log('неверный хеш: ' + calculateHashForBlock(newBlock) + ' ' + newBlock.hash);
        return false;
    }
    return true;
};
