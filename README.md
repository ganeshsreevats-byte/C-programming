# C-programming
just coming to know how to make C programming successful using my moto g35 mobile phone
#include <stdio.h>

int main() {
    float principal;
    float rate;
    int years;
    float final_amount;
    float target_goal;

    printf("--- Fintech Savings Calculator ---\n\n");

    printf("Enter initial investment (Rs): ");
    scanf("%f", &principal);

    printf("Enter interest rate (in %%): ");
    scanf("%f", &rate);

    printf("Enter number of years: ");
    scanf("%d", &years);
    
    printf("Enter target goal (Rs): ");
    scanf("%f", &target_goal);

    // Clean, direct math logic
    final_amount = principal + (principal * (rate / 100) * years);

    printf("\n💰 Calculating returns...\n");
    printf("After %d years, your balance: Rs %.2f\n", years, final_amount);

    if (final_amount >= target_goal) {
        printf("🎉 Goal Achieved!\n");
    } else {
        printf("⚠️ Short of goal by: Rs %.2f\n", target_goal - final_amount);
    }

    return 0;
}
