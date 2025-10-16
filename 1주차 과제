#include <stdio.h>

int main() {
    int product_count;
    int incoming_stock[100];
    int sales_quantity[100];
    int current_stock[100];
    int search_id;

    printf("상품 종류의 개수를 입력하세요 (1~100): ");
    scanf("%d", &product_count);

    printf("상품별 입고 수량을 순서대로 입력하세요: ");
    for (int i = 0; i < product_count; i++) {
        scanf("%d", &incoming_stock[i]);
    }

    printf("상품별 판매 수량을 순서대로 입력하세요: ");
    for (int i = 0; i < product_count; i++) {
        scanf("%d", &sales_quantity[i]);
    }

    for (int i = 0; i < product_count; i++) {
        current_stock[i] = incoming_stock[i] - sales_quantity[i];
    }

    printf("재고를 조회할 상품 ID를 입력하세요: ");
    scanf("%d", &search_id);

    printf("\n--- 재고 현황 ---\n");
    printf("요청하신 ID %d의 재고는 %d개 입니다.\n", search_id, current_stock[search_id - 1]);

    printf("전체 상품 재고: ");
    for (int i = 0; i < product_count; i++) {
        printf("%d ", current_stock[i]);
    }
    printf("\n");

    return 0;
}